# Comparing `tmp/vkdispatch-0.0.2.tar.gz` & `tmp/vkdispatch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vkdispatch-0.0.2.tar", last modified: Wed Apr  3 18:04:20 2024, max compression
+gzip compressed data, was "vkdispatch-0.0.3.tar", last modified: Wed Apr  3 19:24:59 2024, max compression
```

## Comparing `vkdispatch-0.0.2.tar` & `vkdispatch-0.0.3.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.747596 vkdispatch-0.0.2/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11357 2024-04-03 01:33:55.000000 vkdispatch-0.0.2/LICENSE
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1581 2024-04-03 17:52:22.000000 vkdispatch-0.0.2/MANIFEST.in
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      809 2024-04-03 18:04:20.747390 vkdispatch-0.0.2/PKG-INFO
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      121 2024-04-03 01:33:55.000000 vkdispatch-0.0.2/README.md
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.719555 vkdispatch-0.0.2/deps/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.719487 vkdispatch-0.0.2/deps/VKL/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.719416 vkdispatch-0.0.2/deps/VKL/include/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.726022 vkdispatch-0.0.2/deps/VKL/include/VKL/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      553 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKL.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2037 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLBuffer.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2580 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLCommandBuffer.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      829 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLDescriptorSet.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8273 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLDevice.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1384 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLFramebuffer.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2695 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLImage.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      834 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLImageView.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4280 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLInstance.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1482 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLPhysicalDevice.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2240 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLPipeline.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2984 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLPipelineLayout.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1166 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLQueue.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3570 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLRenderPass.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      671 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLStaticAllocator.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1790 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLSurface.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1628 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKLSwapChain.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3975 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/include/VKL/VKL_base.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.730371 vkdispatch-0.0.2/deps/VKL/src/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8143 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLBuffer.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7097 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLCommandBuffer.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3646 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLDescriptorSet.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    24498 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLDevice.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3322 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLFramebuffer.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15023 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLImage.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2433 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLImageView.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11594 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLInstance.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3688 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLPhysicalDevice.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12903 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLPipeline.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12256 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLPipelineLayout.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2421 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLQueue.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6916 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLRenderPass.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3349 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLStaticAllocator.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5516 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLSurface.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    10971 2024-04-03 17:02:02.000000 vkdispatch-0.0.2/deps/VKL/src/VKLSwapChain.cpp
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.719608 vkdispatch-0.0.2/deps/VkFFT/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.730679 vkdispatch-0.0.2/deps/VkFFT/vkFFT/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.722123 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.731334 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12556 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_DeleteApp.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    91082 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_InitializeApp.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    44680 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_RunApp.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.721809 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.732003 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15591 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelStartEnd.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12866 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelUtils.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.721461 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.735857 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9486 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Constants.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    14546 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutput.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6762 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutputLayout.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4342 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_PushConstants.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23925 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Registers.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15546 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_SharedMemory.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.736041 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23235 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/vkFFT_Transfers.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7697 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_Zeropad.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.737347 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.738316 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5753 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_4step.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11508 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Bluestein.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    19521 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Convolution.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    22937 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2C.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   141736 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2R.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    91669 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RaderKernels.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   102595 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixKernels.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    35985 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixShuffle.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    28166 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixStage.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    84118 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_ReadWrite.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6365 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RegisterBoost.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.738875 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12743 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_FFT.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9610 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_R2C_even_decomposition.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.739184 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   114660 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/vkFFT_MathUtils.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.739417 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1722 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/vkFFT_StringManager.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.722059 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.741176 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    33238 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_CompileKernel.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5016 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DeletePlan.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    26535 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DispatchPlan.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    27280 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_InitAPIParameters.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    16495 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_ManageMemory.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    80386 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_UpdateBuffers.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.743647 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    37848 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_AxisBlockSplitter.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   102541 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_ManageLUT.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    73734 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_RecursiveFFTGenerators.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)   147838 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_Scheduler.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.744291 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    50505 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_FFT.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    17441 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_R2C.h
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.744482 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)    58072 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/vkFFT_Structs.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3191 2024-04-03 17:02:14.000000 vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      801 2024-04-03 17:03:45.000000 vkdispatch-0.0.2/pyproject.toml
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       38 2024-04-03 18:04:20.747636 vkdispatch-0.0.2/setup.cfg
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2121 2024-04-03 18:04:14.000000 vkdispatch-0.0.2/setup.py
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.744853 vkdispatch-0.0.2/vkdispatch/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       29 2024-04-03 17:51:26.000000 vkdispatch-0.0.2/vkdispatch/__init__.py
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1578 2024-04-03 17:50:50.000000 vkdispatch-0.0.2/vkdispatch/init.py
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.747151 vkdispatch-0.0.2/vkdispatch.egg-info/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      809 2024-04-03 18:04:20.000000 vkdispatch-0.0.2/vkdispatch.egg-info/PKG-INFO
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5203 2024-04-03 18:04:20.000000 vkdispatch-0.0.2/vkdispatch.egg-info/SOURCES.txt
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)        1 2024-04-03 18:04:20.000000 vkdispatch-0.0.2/vkdispatch.egg-info/dependency_links.txt
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)        1 2024-04-03 01:55:16.000000 vkdispatch-0.0.2/vkdispatch.egg-info/not-zip-safe
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       23 2024-04-03 18:04:20.000000 vkdispatch-0.0.2/vkdispatch.egg-info/requires.txt
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)       29 2024-04-03 18:04:20.000000 vkdispatch-0.0.2/vkdispatch.egg-info/top_level.txt
-drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 18:04:20.746965 vkdispatch-0.0.2/vkdispatch_native/
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      289 2024-04-03 17:46:08.000000 vkdispatch-0.0.2/vkdispatch_native/base.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1736 2024-04-03 17:48:25.000000 vkdispatch-0.0.2/vkdispatch_native/init.cpp
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      402 2024-04-03 17:45:16.000000 vkdispatch-0.0.2/vkdispatch_native/init.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1329 2024-04-03 17:45:04.000000 vkdispatch-0.0.2/vkdispatch_native/init_wrapper.pxd
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      432 2024-04-03 17:49:09.000000 vkdispatch-0.0.2/vkdispatch_native/internal.h
--rw-r--r--   0 shaharsandhaus   (501) staff       (20)      164 2024-04-03 17:44:45.000000 vkdispatch-0.0.2/vkdispatch_native/wrapper.pyx
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.225972 vkdispatch-0.0.3/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11357 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/LICENSE
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1581 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/MANIFEST.in
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      809 2024-04-03 19:24:59.225772 vkdispatch-0.0.3/PKG-INFO
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      121 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/README.md
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.201936 vkdispatch-0.0.3/deps/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.201848 vkdispatch-0.0.3/deps/VKL/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.201772 vkdispatch-0.0.3/deps/VKL/include/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.205981 vkdispatch-0.0.3/deps/VKL/include/VKL/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      553 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKL.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2037 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLBuffer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2580 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLCommandBuffer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      829 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLDescriptorSet.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8273 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLDevice.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1384 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLFramebuffer.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2695 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLImage.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      834 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLImageView.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4280 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLInstance.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1482 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLPhysicalDevice.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2240 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLPipeline.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2984 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLPipelineLayout.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1166 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLQueue.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3570 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLRenderPass.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      671 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLStaticAllocator.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1790 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLSurface.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1628 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKLSwapChain.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3975 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/include/VKL/VKL_base.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.208360 vkdispatch-0.0.3/deps/VKL/src/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     8143 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLBuffer.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7097 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLCommandBuffer.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3646 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLDescriptorSet.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    24498 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLDevice.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3322 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLFramebuffer.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15023 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLImage.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2433 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLImageView.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11594 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLInstance.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3688 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLPhysicalDevice.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12903 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLPipeline.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12219 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLPipelineLayout.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2421 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLQueue.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6916 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLRenderPass.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3383 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLStaticAllocator.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5516 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLSurface.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    10971 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VKL/src/VKLSwapChain.cpp
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.201990 vkdispatch-0.0.3/deps/VkFFT/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.208526 vkdispatch-0.0.3/deps/VkFFT/vkFFT/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.202939 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.208920 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12556 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_DeleteApp.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    91082 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_InitializeApp.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    44680 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_RunApp.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.202667 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.209370 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15591 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelStartEnd.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12866 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelUtils.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.202379 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.210229 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9486 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Constants.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    14546 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutput.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6762 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutputLayout.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     4342 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_PushConstants.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23925 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Registers.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    15546 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_SharedMemory.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.210389 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    23235 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/vkFFT_Transfers.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     7697 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_Zeropad.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.219662 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.220584 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5753 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_4step.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    11508 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Bluestein.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    19521 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Convolution.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    22937 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2C.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   141736 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2R.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    91669 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RaderKernels.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   102595 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixKernels.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    35985 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixShuffle.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    28166 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixStage.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    84118 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_ReadWrite.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     6365 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RegisterBoost.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.221118 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    12743 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_FFT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     9610 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_R2C_even_decomposition.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.221314 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   114660 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/vkFFT_MathUtils.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.221478 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1722 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/vkFFT_StringManager.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.202875 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.222324 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    33238 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_CompileKernel.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5016 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DeletePlan.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    26535 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DispatchPlan.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    27280 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_InitAPIParameters.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    16495 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_ManageMemory.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    80386 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_UpdateBuffers.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.222952 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    37848 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_AxisBlockSplitter.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   102541 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_ManageLUT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    73734 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_RecursiveFFTGenerators.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)   147838 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_Scheduler.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.223375 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    50505 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_FFT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    17441 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_R2C.h
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.223559 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)    58072 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/vkFFT_Structs.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     3191 2024-04-03 19:21:47.000000 vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      801 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/pyproject.toml
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       38 2024-04-03 19:24:59.226008 vkdispatch-0.0.3/setup.cfg
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     2351 2024-04-03 19:23:31.000000 vkdispatch-0.0.3/setup.py
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.223823 vkdispatch-0.0.3/vkdispatch/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       51 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/vkdispatch/__init__.py
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1578 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/vkdispatch/init.py
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.225313 vkdispatch-0.0.3/vkdispatch.egg-info/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      809 2024-04-03 19:24:59.000000 vkdispatch-0.0.3/vkdispatch.egg-info/PKG-INFO
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     5203 2024-04-03 19:24:59.000000 vkdispatch-0.0.3/vkdispatch.egg-info/SOURCES.txt
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)        1 2024-04-03 19:24:59.000000 vkdispatch-0.0.3/vkdispatch.egg-info/dependency_links.txt
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)        1 2024-04-03 19:22:33.000000 vkdispatch-0.0.3/vkdispatch.egg-info/not-zip-safe
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       23 2024-04-03 19:24:59.000000 vkdispatch-0.0.3/vkdispatch.egg-info/requires.txt
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)       29 2024-04-03 19:24:59.000000 vkdispatch-0.0.3/vkdispatch.egg-info/top_level.txt
+drwxr-xr-x   0 shaharsandhaus   (501) staff       (20)        0 2024-04-03 19:24:59.225177 vkdispatch-0.0.3/vkdispatch_native/
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      289 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/vkdispatch_native/base.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1736 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/vkdispatch_native/init.cpp
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      402 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/vkdispatch_native/init.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)     1329 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/vkdispatch_native/init_wrapper.pxd
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      432 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/vkdispatch_native/internal.h
+-rw-r--r--   0 shaharsandhaus   (501) staff       (20)      164 2024-04-03 19:21:33.000000 vkdispatch-0.0.3/vkdispatch_native/wrapper.pyx
```

### Comparing `vkdispatch-0.0.2/LICENSE` & `vkdispatch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/MANIFEST.in` & `vkdispatch-0.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/PKG-INFO` & `vkdispatch-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vkdispatch
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python module for orchestrating and dispatching large computations across multi-GPU systems using Vulkan.
 Author-email: Shahar Sandhaus <shahar.sandhaus@gmail.com>
 Project-URL: Homepage, https://github.com/sharhar/vkdispatch
 Project-URL: Issues, https://github.com/sharhar/vkdispatch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKL.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKL.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKLBuffer.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLBuffer.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKLCommandBuffer.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLCommandBuffer.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKLDescriptorSet.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLDescriptorSet.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKLDevice.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLDevice.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKLFramebuffer.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLFramebuffer.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKLImage.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLImage.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKLImageView.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLImageView.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKLInstance.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLInstance.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKLPhysicalDevice.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLPhysicalDevice.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKLPipeline.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLPipeline.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKLPipelineLayout.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLPipelineLayout.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKLQueue.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLQueue.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKLRenderPass.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLRenderPass.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKLStaticAllocator.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLStaticAllocator.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKLSurface.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLSurface.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKLSwapChain.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKLSwapChain.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/include/VKL/VKL_base.h` & `vkdispatch-0.0.3/deps/VKL/include/VKL/VKL_base.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/src/VKLBuffer.cpp` & `vkdispatch-0.0.3/deps/VKL/src/VKLBuffer.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/src/VKLCommandBuffer.cpp` & `vkdispatch-0.0.3/deps/VKL/src/VKLCommandBuffer.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/src/VKLDescriptorSet.cpp` & `vkdispatch-0.0.3/deps/VKL/src/VKLDescriptorSet.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/src/VKLDevice.cpp` & `vkdispatch-0.0.3/deps/VKL/src/VKLDevice.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/src/VKLFramebuffer.cpp` & `vkdispatch-0.0.3/deps/VKL/src/VKLFramebuffer.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/src/VKLImage.cpp` & `vkdispatch-0.0.3/deps/VKL/src/VKLImage.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/src/VKLImageView.cpp` & `vkdispatch-0.0.3/deps/VKL/src/VKLImageView.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/src/VKLInstance.cpp` & `vkdispatch-0.0.3/deps/VKL/src/VKLInstance.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/src/VKLPhysicalDevice.cpp` & `vkdispatch-0.0.3/deps/VKL/src/VKLPhysicalDevice.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/src/VKLPipeline.cpp` & `vkdispatch-0.0.3/deps/VKL/src/VKLPipeline.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/src/VKLPipelineLayout.cpp` & `vkdispatch-0.0.3/deps/VKL/src/VKLPipelineLayout.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -141,29 +141,28 @@
 	m_shaderModuleCreateInfos.push_back(result);
 	
 	return invalidate();
 	
 }
 
 uint32_t* util_compile_shader_code(glslang_stage_t stage, size_t* size, const char* shader_source, const char* shader_name) {
-    const glslang_input_t input = {
-        .language = GLSLANG_SOURCE_GLSL,
-        .stage = stage,
-        .client = GLSLANG_CLIENT_VULKAN,
-        .client_version = GLSLANG_TARGET_VULKAN_1_2,
-        .target_language = GLSLANG_TARGET_SPV,
-        .target_language_version = GLSLANG_TARGET_SPV_1_0,
-        .code = shader_source,
-        .default_version = 100,
-        .default_profile = GLSLANG_NO_PROFILE,
-        .force_default_version_and_profile = false,
-        .forward_compatible = false,
-        .messages = GLSLANG_MSG_DEFAULT_BIT,
-        .resource = glslang_default_resource(),
-    };
+    glslang_input_t input = {};
+	input.language = GLSLANG_SOURCE_GLSL;
+	input.stage = stage;
+	input.client = GLSLANG_CLIENT_VULKAN;
+	input.client_version = GLSLANG_TARGET_VULKAN_1_2;
+	input.target_language = GLSLANG_TARGET_SPV;
+	input.target_language_version = GLSLANG_TARGET_SPV_1_0;
+	input.code = shader_source;
+	input.default_version = 100;
+	input.default_profile = GLSLANG_NO_PROFILE;
+	input.force_default_version_and_profile = false;
+	input.forward_compatible = false;
+	input.messages = GLSLANG_MSG_DEFAULT_BIT;
+	input.resource = glslang_default_resource();
 
     glslang_shader_t* shader = glslang_shader_create(&input);
 
     if (!glslang_shader_preprocess(shader, &input))	{
         LOG_ERROR("GLSL preprocessing failed %s", shader_name);
         LOG_ERROR("%s", glslang_shader_get_info_log(shader));
         LOG_ERROR("%s", glslang_shader_get_info_debug_log(shader));
```

### Comparing `vkdispatch-0.0.2/deps/VKL/src/VKLQueue.cpp` & `vkdispatch-0.0.3/deps/VKL/src/VKLQueue.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/src/VKLRenderPass.cpp` & `vkdispatch-0.0.3/deps/VKL/src/VKLRenderPass.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/src/VKLStaticAllocator.cpp` & `vkdispatch-0.0.3/deps/VKL/src/VKLStaticAllocator.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,16 @@
     uint32_t memoryTypeBits = 0xffffffff;
     for (int i = 0; i < m_requirements.size(); i++) {
         memoryTypeBits &= m_requirements[i].memoryTypeBits;
     }
 
     m_size = 0;
 
-    VkDeviceSize og_sizes[m_requirements.size()];
+    std::vector<VkDeviceSize> og_sizes;
+    og_sizes.resize(m_requirements.size());
 
     for (int i = 0; i < m_requirements.size(); i++) {
         og_sizes[i] = m_requirements[i].size;
 
         if(m_requirements[i].size % m_requirements[i].alignment != 0)
             m_requirements[i].size = (1 + (m_requirements[i].size / m_requirements[i].alignment)) * m_requirements[i].alignment;
```

### Comparing `vkdispatch-0.0.2/deps/VKL/src/VKLSurface.cpp` & `vkdispatch-0.0.3/deps/VKL/src/VKLSurface.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VKL/src/VKLSwapChain.cpp` & `vkdispatch-0.0.3/deps/VKL/src/VKLSwapChain.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_DeleteApp.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_DeleteApp.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_InitializeApp.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_InitializeApp.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_RunApp.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_AppManagement/vkFFT_RunApp.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelStartEnd.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelStartEnd.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelUtils.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_KernelUtils.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Constants.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Constants.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutput.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutput.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutputLayout.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_InputOutputLayout.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_PushConstants.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_PushConstants.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Registers.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_Registers.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_SharedMemory.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryInitialization/vkFFT_SharedMemory.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/vkFFT_Transfers.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_MemoryManagement/vkFFT_MemoryTransfers/vkFFT_Transfers.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_Zeropad.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel0/vkFFT_Zeropad.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_4step.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_4step.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Bluestein.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Bluestein.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Convolution.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_Convolution.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2C.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2C.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2R.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/PrePostProcessing/vkFFT_R2R.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RaderKernels.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RaderKernels.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixKernels.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixKernels.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixShuffle.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixShuffle.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixStage.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RadixStage.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_ReadWrite.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_ReadWrite.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RegisterBoost.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel1/vkFFT_RegisterBoost.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_FFT.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_FFT.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_R2C_even_decomposition.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_KernelsLevel2/vkFFT_R2C_even_decomposition.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/vkFFT_MathUtils.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_MathUtils/vkFFT_MathUtils.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/vkFFT_StringManager.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_CodeGen/vkFFT_StringManagement/vkFFT_StringManager.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_CompileKernel.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_CompileKernel.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DeletePlan.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DeletePlan.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DispatchPlan.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_DispatchPlan.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_InitAPIParameters.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_InitAPIParameters.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_ManageMemory.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_ManageMemory.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_UpdateBuffers.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_API_handles/vkFFT_UpdateBuffers.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_AxisBlockSplitter.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_AxisBlockSplitter.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_ManageLUT.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_ManageLUT.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_RecursiveFFTGenerators.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_RecursiveFFTGenerators.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_Scheduler.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_HostFunctions/vkFFT_Scheduler.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_FFT.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_FFT.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_R2C.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_PlanManagement/vkFFT_Plans/vkFFT_Plan_R2C.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/vkFFT_Structs.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT/vkFFT_Structs/vkFFT_Structs.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/deps/VkFFT/vkFFT/vkFFT.h` & `vkdispatch-0.0.3/deps/VkFFT/vkFFT/vkFFT.h`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/pyproject.toml` & `vkdispatch-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "Cython",
     "numpy"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vkdispatch"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Shahar Sandhaus", email="shahar.sandhaus@gmail.com" },
 ]
 description = "A Python module for orchestrating and dispatching large computations across multi-GPU systems using Vulkan."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `vkdispatch-0.0.2/setup.py` & `vkdispatch-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from setuptools import setup
-from distutils.extension import Extension
+from setuptools import setup, Extension
 import numpy
 import os
 
 try:
     numpy_include = numpy.get_include()
 except AttributeError:
     numpy_include = numpy.get_numpy_include()
@@ -41,27 +40,41 @@
     'deps/VKL/src/VKLQueue.cpp',
     'deps/VKL/src/VKLRenderPass.cpp',
     'deps/VKL/src/VKLSurface.cpp',
     'deps/VKL/src/VKLStaticAllocator.cpp',
     'deps/VKL/src/VKLSwapChain.cpp'
 ]
 
+vulkan_lib_dir = vulkan_root + '/lib'
+
+unix_libs = ['dl', 'pthread', 'vulkan']
+windows_libs = ['vulkan-1']
+
+platform_libs = unix_libs if os.name == 'posix' else windows_libs
+
+compile_libs = platform_libs + ['glslang', 'SPIRV', 'MachineIndependent', 'GenericCodeGen']
+for file in os.listdir(vulkan_lib_dir):
+    if "OGLCompiler" in file:
+        compile_libs.append('OGLCompiler')
+        break
+
+compile_libs.extend(['OSDependent', 'SPIRV-Tools', 'SPIRV-Tools-opt',
+                             'SPIRV-Tools-link', 'SPIRV-Tools-reduce',
+                             'glslang-default-resource-limits'])
+
+
 setup(
     name='vkdispatch',
     packages=['vkdispatch'],
     ext_modules=[
         Extension('vkdispatch_native',
                   sources=sources,
                   language='c++',
-                  library_dirs=[vulkan_root + '/lib'],
-                  libraries=['dl', 'pthread', 'vulkan', 'glslang', 'SPIRV', 
-                             'MachineIndependent', 'GenericCodeGen', # 'OGLCompiler', 
-                             'OSDependent', 'SPIRV-Tools', 'SPIRV-Tools-opt',
-                             'SPIRV-Tools-link', 'SPIRV-Tools-reduce',
-                             'glslang-default-resource-limits'],
+                  library_dirs=[vulkan_lib_dir],
+                  libraries=compile_libs,
                   extra_compile_args=['-g', '-std=c++11'],
                   extra_link_args=['-g', f'-Wl,-rpath,{vulkan_root}/lib'],
                   include_dirs=include_directories
         )
     ],
     zip_safe=False
 )
```

### Comparing `vkdispatch-0.0.2/vkdispatch/init.py` & `vkdispatch-0.0.3/vkdispatch/init.py`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/vkdispatch.egg-info/PKG-INFO` & `vkdispatch-0.0.3/vkdispatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vkdispatch
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python module for orchestrating and dispatching large computations across multi-GPU systems using Vulkan.
 Author-email: Shahar Sandhaus <shahar.sandhaus@gmail.com>
 Project-URL: Homepage, https://github.com/sharhar/vkdispatch
 Project-URL: Issues, https://github.com/sharhar/vkdispatch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vkdispatch-0.0.2/vkdispatch.egg-info/SOURCES.txt` & `vkdispatch-0.0.3/vkdispatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/vkdispatch_native/init.cpp` & `vkdispatch-0.0.3/vkdispatch_native/init.cpp`

 * *Files identical despite different names*

### Comparing `vkdispatch-0.0.2/vkdispatch_native/init_wrapper.pxd` & `vkdispatch-0.0.3/vkdispatch_native/init_wrapper.pxd`

 * *Files identical despite different names*

