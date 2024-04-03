# Comparing `tmp/vkdispatch-0.0.1.tar.gz` & `tmp/vkdispatch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vkdispatch-0.0.1.tar", last modified: Wed Apr  3 01:55:16 2024, max compression
+gzip compressed data, was "vkdispatch-0.0.2.tar", last modified: Wed Apr  3 18:04:20 2024, max compression
```

## Comparing `vkdispatch-0.0.1.tar` & `vkdispatch-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,125 @@
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 01:55:16.983928 vkdispatch-0.0.1/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11357 2024-04-03 01:33:55.000000 vkdispatch-0.0.1/LICENSE
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       29 2024-04-03 01:45:03.000000 vkdispatch-0.0.1/MANIFEST.in
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      809 2024-04-03 01:55:16.983700 vkdispatch-0.0.1/PKG-INFO
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      121 2024-04-03 01:33:55.000000 vkdispatch-0.0.1/README.md
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      801 2024-04-03 01:46:56.000000 vkdispatch-0.0.1/pyproject.toml
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       38 2024-04-03 01:55:16.983969 vkdispatch-0.0.1/setup.cfg
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      774 2024-04-03 01:48:02.000000 vkdispatch-0.0.1/setup.py
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 01:55:16.981675 vkdispatch-0.0.1/vkdispatch/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       22 2024-04-02 20:54:31.000000 vkdispatch-0.0.1/vkdispatch/__init__.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       43 2024-04-02 02:34:56.000000 vkdispatch-0.0.1/vkdispatch/example.py
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 01:55:16.983476 vkdispatch-0.0.1/vkdispatch.egg-info/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      809 2024-04-03 01:55:16.000000 vkdispatch-0.0.1/vkdispatch.egg-info/PKG-INFO
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      382 2024-04-03 01:55:16.000000 vkdispatch-0.0.1/vkdispatch.egg-info/SOURCES.txt
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)        1 2024-04-03 01:55:16.000000 vkdispatch-0.0.1/vkdispatch.egg-info/dependency_links.txt
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)        1 2024-04-03 01:55:16.000000 vkdispatch-0.0.1/vkdispatch.egg-info/not-zip-safe
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       23 2024-04-03 01:55:16.000000 vkdispatch-0.0.1/vkdispatch.egg-info/requires.txt
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       29 2024-04-03 01:55:16.000000 vkdispatch-0.0.1/vkdispatch.egg-info/top_level.txt
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 01:55:16.983189 vkdispatch-0.0.1/vkdispatch_native/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       60 2024-04-02 22:09:44.000000 vkdispatch-0.0.1/vkdispatch_native/init.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       99 2024-04-02 22:09:26.000000 vkdispatch-0.0.1/vkdispatch_native/init.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      266 2024-04-02 22:44:18.000000 vkdispatch-0.0.1/vkdispatch_native/wrapper.pyx
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.747596 vkdispatch-0.0.2/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11357 2024-04-03 01:33:55.000000 vkdispatch-0.0.2/LICENSE
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1581 2024-04-03 17:52:22.000000 vkdispatch-0.0.2/MANIFEST.in
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      809 2024-04-03 18:04:20.747390 vkdispatch-0.0.2/PKG-INFO
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      121 2024-04-03 01:33:55.000000 vkdispatch-0.0.2/README.md
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.719555 vkdispatch-0.0.2/deps/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.719487 vkdispatch-0.0.2/deps/VKL/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.719416 vkdispatch-0.0.2/deps/VKL/include/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.726022 vkdispatch-0.0.2/deps/VKL/include/VKL/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      553 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKL.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2037 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLBuffer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2580 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLCommandBuffer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      829 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLDescriptorSet.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8273 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLDevice.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1384 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLFramebuffer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2695 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLImage.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      834 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLImageView.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4280 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLInstance.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1482 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLPhysicalDevice.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2240 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLPipeline.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2984 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLPipelineLayout.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1166 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLQueue.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3570 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLRenderPass.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      671 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLStaticAllocator.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1790 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLSurface.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1628 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLSwapChain.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3975 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKL_base.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.730371 vkdispatch-0.0.2/deps/VKL/src/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8143 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLBuffer.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7097 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLCommandBuffer.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3646 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLDescriptorSet.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    24498 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLDevice.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3322 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLFramebuffer.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15023 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLImage.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2433 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLImageView.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11594 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLInstance.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3688 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLPhysicalDevice.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12903 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLPipeline.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12256 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLPipelineLayout.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2421 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLQueue.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6916 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLRenderPass.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3349 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLStaticAllocator.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5516 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLSurface.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    10971 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLSwapChain.cpp
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.719608 vkdispatch-0.0.2/deps/VkFFT/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.730679 vkdispatch-0.0.2/deps/VkFFT/vkFFT/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.722123 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.731334 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12556 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_DeleteApp.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    91082 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_InitializeApp.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    44680 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_RunApp.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.721809 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.732003 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15591 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelStartEnd.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12866 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelUtils.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.721461 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.735857 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9486 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Constants.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    14546 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutput.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6762 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutputLayout.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4342 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_PushConstants.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23925 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Registers.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15546 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_SharedMemory.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.736041 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23235 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/vkFFT_Transfers.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7697 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_Zeropad.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.737347 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.738316 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5753 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_4step.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11508 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Bluestein.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    19521 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Convolution.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    22937 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2C.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   141736 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2R.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    91669 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RaderKernels.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   102595 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixKernels.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    35985 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixShuffle.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    28166 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixStage.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    84118 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_ReadWrite.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6365 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RegisterBoost.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.738875 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12743 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_FFT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9610 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_R2C_even_decomposition.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.739184 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   114660 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/vkFFT_MathUtils.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.739417 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1722 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/vkFFT_StringManager.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.722059 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.741176 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    33238 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_CompileKernel.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5016 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DeletePlan.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    26535 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DispatchPlan.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    27280 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_InitAPIParameters.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    16495 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_ManageMemory.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    80386 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_UpdateBuffers.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.743647 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    37848 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_AxisBlockSplitter.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   102541 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_ManageLUT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    73734 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_RecursiveFFTGenerators.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   147838 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_Scheduler.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.744291 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    50505 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_FFT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    17441 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_R2C.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.744482 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    58072 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/vkFFT_Structs.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3191 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      801 2024-04-03 17:03:45.000000 vkdispatch-0.0.2/pyproject.toml
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       38 2024-04-03 18:04:20.747636 vkdispatch-0.0.2/setup.cfg
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2121 2024-04-03 18:04:14.000000 vkdispatch-0.0.2/setup.py
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.744853 vkdispatch-0.0.2/vkdispatch/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       29 2024-04-03 17:51:26.000000 vkdispatch-0.0.2/vkdispatch/__init__.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1578 2024-04-03 17:50:50.000000 vkdispatch-0.0.2/vkdispatch/init.py
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.747151 vkdispatch-0.0.2/vkdispatch.egg-info/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      809 2024-04-03 18:04:20.000000 vkdispatch-0.0.2/vkdispatch.egg-info/PKG-INFO
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5203 2024-04-03 18:04:20.000000 vkdispatch-0.0.2/vkdispatch.egg-info/SOURCES.txt
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)        1 2024-04-03 18:04:20.000000 vkdispatch-0.0.2/vkdispatch.egg-info/dependency_links.txt
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)        1 2024-04-03 01:55:16.000000 vkdispatch-0.0.2/vkdispatch.egg-info/not-zip-safe
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       23 2024-04-03 18:04:20.000000 vkdispatch-0.0.2/vkdispatch.egg-info/requires.txt
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       29 2024-04-03 18:04:20.000000 vkdispatch-0.0.2/vkdispatch.egg-info/top_level.txt
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.746965 vkdispatch-0.0.2/vkdispatch_native/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      289 2024-04-03 17:46:08.000000 vkdispatch-0.0.2/vkdispatch_native/base.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1736 2024-04-03 17:48:25.000000 vkdispatch-0.0.2/vkdispatch_native/init.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      402 2024-04-03 17:45:16.000000 vkdispatch-0.0.2/vkdispatch_native/init.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1329 2024-04-03 17:45:04.000000 vkdispatch-0.0.2/vkdispatch_native/init_wrapper.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      432 2024-04-03 17:49:09.000000 vkdispatch-0.0.2/vkdispatch_native/internal.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      164 2024-04-03 17:44:45.000000 vkdispatch-0.0.2/vkdispatch_native/wrapper.pyx
```

### Comparing `vkdispatch-0.0.1/LICENSE` & `vkdispatch-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.1/PKG-INFO` & `vkdispatch-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vkdispatch
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python module for orchestrating and dispatching large computations across multi-GPU systems using Vulkan.
 Author-email: Shahar Sandhaus <shahar.sandhaus@gmail.com>
 Project-URL: Homepage, https://github.com/sharhar/vkdispatch
 Project-URL: Issues, https://github.com/sharhar/vkdispatch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vkdispatch-0.0.1/pyproject.toml` & `vkdispatch-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "Cython",
     "numpy"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vkdispatch"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Shahar Sandhaus", email="shahar.sandhaus@gmail.com" },
 ]
 description = "A Python module for orchestrating and dispatching large computations across multi-GPU systems using Vulkan."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `vkdispatch-0.0.1/vkdispatch.egg-info/PKG-INFO` & `vkdispatch-0.0.2/vkdispatch.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vkdispatch
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python module for orchestrating and dispatching large computations across multi-GPU systems using Vulkan.
 Author-email: Shahar Sandhaus <shahar.sandhaus@gmail.com>
 Project-URL: Homepage, https://github.com/sharhar/vkdispatch
 Project-URL: Issues, https://github.com/sharhar/vkdispatch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

