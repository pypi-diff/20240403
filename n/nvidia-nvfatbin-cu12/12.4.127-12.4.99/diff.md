# Comparing `tmp/nvidia_nvfatbin_cu12-12.4.127-py3-none-manylinux2014_x86_64.whl.zip` & `tmp/nvidia_nvfatbin_cu12-12.4.99-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,15 @@
-Zip file size: 932214 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-15 22:50 nvidia/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-15 22:50 nvidia/nvfatbin/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-15 22:50 nvidia/nvfatbin/include/__init__.py
--rw-r--r--  2.0 unx     9597 b- defN 24-Mar-15 22:50 nvidia/nvfatbin/include/nvFatbin.h
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-15 22:50 nvidia/nvfatbin/lib/__init__.py
--rw-r--r--  2.0 unx  2381192 b- defN 24-Mar-15 22:50 nvidia/nvfatbin/lib/libnvfatbin.so.12
--rw-r--r--  2.0 unx    59262 b- defN 24-Mar-15 22:50 nvidia_nvfatbin_cu12-12.4.127.dist-info/License.txt
--rw-r--r--  2.0 unx     1537 b- defN 24-Mar-15 22:50 nvidia_nvfatbin_cu12-12.4.127.dist-info/METADATA
--rw-r--r--  2.0 unx      109 b- defN 24-Mar-15 22:50 nvidia_nvfatbin_cu12-12.4.127.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Mar-15 22:50 nvidia_nvfatbin_cu12-12.4.127.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      986 b- defN 24-Mar-15 22:50 nvidia_nvfatbin_cu12-12.4.127.dist-info/RECORD
-11 files, 2452690 bytes uncompressed, 930506 bytes compressed:  62.1%
+Zip file size: 1556840 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-28 02:55 nvidia/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-28 02:55 nvidia/nvfatbin/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-28 02:55 nvidia/nvfatbin/bin/__init__.py
+-rw-r--r--  2.0 unx   749056 b- defN 24-Feb-28 02:55 nvidia/nvfatbin/bin/nvfatbin_120_0.dll
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-28 02:55 nvidia/nvfatbin/include/__init__.py
+-rw-r--r--  2.0 unx     9868 b- defN 24-Feb-28 02:55 nvidia/nvfatbin/include/nvFatbin.h
+-rw-r--r--  2.0 unx     3560 b- defN 24-Feb-28 02:55 nvidia/nvfatbin/lib/x64/nvfatbin.lib
+-rw-r--r--  2.0 unx  4004312 b- defN 24-Feb-28 02:55 nvidia/nvfatbin/lib/x64/nvfatbin_static.lib
+-rw-r--r--  2.0 unx    59262 b- defN 24-Feb-28 02:55 nvidia_nvfatbin_cu12-12.4.99.dist-info/License.txt
+-rw-r--r--  2.0 unx     1536 b- defN 24-Feb-28 02:55 nvidia_nvfatbin_cu12-12.4.99.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 24-Feb-28 02:55 nvidia_nvfatbin_cu12-12.4.99.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Feb-28 02:55 nvidia_nvfatbin_cu12-12.4.99.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1176 b- defN 24-Feb-28 02:55 nvidia_nvfatbin_cu12-12.4.99.dist-info/RECORD
+13 files, 4828875 bytes uncompressed, 1554830 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -1,34 +1,40 @@
 Filename: nvidia/__init__.py
 Comment: 
 
 Filename: nvidia/nvfatbin/__init__.py
 Comment: 
 
+Filename: nvidia/nvfatbin/bin/__init__.py
+Comment: 
+
+Filename: nvidia/nvfatbin/bin/nvfatbin_120_0.dll
+Comment: 
+
 Filename: nvidia/nvfatbin/include/__init__.py
 Comment: 
 
 Filename: nvidia/nvfatbin/include/nvFatbin.h
 Comment: 
 
-Filename: nvidia/nvfatbin/lib/__init__.py
+Filename: nvidia/nvfatbin/lib/x64/nvfatbin.lib
 Comment: 
 
-Filename: nvidia/nvfatbin/lib/libnvfatbin.so.12
+Filename: nvidia/nvfatbin/lib/x64/nvfatbin_static.lib
 Comment: 
 
-Filename: nvidia_nvfatbin_cu12-12.4.127.dist-info/License.txt
+Filename: nvidia_nvfatbin_cu12-12.4.99.dist-info/License.txt
 Comment: 
 
-Filename: nvidia_nvfatbin_cu12-12.4.127.dist-info/METADATA
+Filename: nvidia_nvfatbin_cu12-12.4.99.dist-info/METADATA
 Comment: 
 
-Filename: nvidia_nvfatbin_cu12-12.4.127.dist-info/WHEEL
+Filename: nvidia_nvfatbin_cu12-12.4.99.dist-info/WHEEL
 Comment: 
 
-Filename: nvidia_nvfatbin_cu12-12.4.127.dist-info/top_level.txt
+Filename: nvidia_nvfatbin_cu12-12.4.99.dist-info/top_level.txt
 Comment: 
 
-Filename: nvidia_nvfatbin_cu12-12.4.127.dist-info/RECORD
+Filename: nvidia_nvfatbin_cu12-12.4.99.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nvidia/nvfatbin/include/nvFatbin.h

 * *Ordering differences only*

```diff
@@ -1,272 +1,272 @@
-/*
- * NVIDIA_COPYRIGHT_BEGIN
- *
- * Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
- *
- * NVIDIA CORPORATION and its licensors retain all intellectual property
- * and proprietary rights in and to this software, related documentation
- * and any modifications thereto.  Any use, reproduction, disclosure or
- * distribution of this software and related documentation without an express
- * license agreement from NVIDIA CORPORATION is strictly prohibited.
- *
- * NVIDIA_COPYRIGHT_END
- */
-
-//
-// nvFatbin.h
-//
-
-#include <stddef.h>
-
-#ifndef nvFatbin_INCLUDED
-#define nvFatbin_INCLUDED
-
-#ifdef __cplusplus
-extern "C"
-{
-#endif
-
-/**
- *
- * \defgroup error Error codes
- *
- */
-
-/** \ingroup error
- *
- * \brief    The enumerated type nvFatbinResult defines API call result codes.
- *           nvFatbin APIs return nvFatbinResult codes to indicate the result.
- */
-
-typedef enum
-{
-  NVFATBIN_SUCCESS = 0,
-  NVFATBIN_ERROR_INTERNAL,
-  NVFATBIN_ERROR_ELF_ARCH_MISMATCH,
-  NVFATBIN_ERROR_ELF_SIZE_MISMATCH,
-  NVFATBIN_ERROR_MISSING_PTX_VERSION,
-  NVFATBIN_ERROR_NULL_POINTER,
-  NVFATBIN_ERROR_COMPRESSION_FAILED,
-  NVFATBIN_ERROR_COMPRESSED_SIZE_EXCEEDED,
-  NVFATBIN_ERROR_UNRECOGNIZED_OPTION,
-  NVFATBIN_ERROR_INVALID_ARCH,
-  NVFATBIN_ERROR_INVALID_NVVM,
-  NVFATBIN_ERROR_EMPTY_INPUT,
-} nvFatbinResult;
-
-/**
- * \ingroup error
- * \brief   nvFatbinGetErrorString returns an error description string for each error code.
- *
- * \param   [in] result       error code
- * \return
- *   - nullptr, if result is NVFATBIN_SUCCESS
- *   - a string, if result is not NVFATBIN_SUCCESS
- *
- */
-const char *nvFatbinGetErrorString(nvFatbinResult result);
-
-/**
- *
- * \defgroup creation Fatbinary Creation
- *
- */
-
-/**
- * \ingroup creation
- * \brief   nvFatbinHandle is the unit of fatbin creation, and an opaque handle for
- *          a program.
- *
- * To create a fatbin, an instance of nvFatbinHandle must be created first with
- * nvFatbinCreate().
- */
-
-typedef struct _nvFatbinHandle *nvFatbinHandle;
-
-/**
- * \defgroup options Supported Options
- *
- * nvFatbin supports the options below.
- * Option names are prefixed with a single dash (\c -).
- * Options that take a value have an assignment operator (\c =)
- * followed by the option value, with no spaces, e.g. \c "-host=windows".
- *
- * The supported options are:
- * - \c -32 \n
- *   Make entries 32 bit.
- * - \c -64 \n
- *   Make entries 64 bit.
- * - \c -c \n
- *   Make relocatable fatbin.
- * - \c -compress=<bool\> \n
- *   Enable (true) / disable (false) compression (default: true).
- * - \c -compress-all \n
- *   Compress everything in the fatbin, even if it's small.
- * - \c -cuda \n
- *   Specify CUDA (rather than OpenCL).
- * - \c -g \n
- *   Generate debug information.
- * - \c -host=<name\> \n
- *   Specify host operating system. Valid options are "linux", "windows", and "mac" (deprecated).
- * - \c -opencl \n
- *   Specify OpenCL (rather than CUDA).
- */
-
-/**
- * \ingroup creation
- * \brief   nvFatbinCreate creates a new handle
- *
- * \param    [out] handle_indirect  Address of nvFatbin handle
- * \param    [in] options       An array of strings, each containing a single option.
- * \param    [in] optionsCount  Number of options.
- * \return
- *   - \link #nvFatbinResult NVFATBIN_SUCCESS \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_NULL_POINTER \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_UNRECOGNIZED_OPTION \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_INTERNAL \endlink
- *
- */
-nvFatbinResult nvFatbinCreate(nvFatbinHandle *handle_indirect, const char **options, size_t optionsCount);
-
-/**
- * \ingroup creation
- * \brief   nvFatbinDestroy destroys the handle.
- *
- * \param    [in] handle_indirect  Pointer to the handle.
- * \return
- *   - \link #nvFatbinResult NVFATBIN_SUCCESS \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_NULL_POINTER \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_INTERNAL \endlink
- *
- * Use of any other pointers to the handle after calling this will result in undefined behavior.
- * The passed in handle will be set to nullptr.
- */
-nvFatbinResult nvFatbinDestroy(nvFatbinHandle *handle_indirect);
-
-/**
- * \ingroup creation
- * \brief   nvFatbinAddPtx adds PTX to the fatbinary.
- *
- * \param    [in] handle      nvFatbin handle.
- * \param    [in] code        The PTX code.
- * \param    [in] size        The size of the PTX code.
- * \param    [in] arch        The architecture that this PTX is for.
- * \param    [in] identifier  Name of the PTX, useful when extracting the fatbin with tools like cuobjdump.
- * \param    [in] optionsCmdLine  Options used during JIT compilation.
- *
- * \return
- *   - \link #nvFatbinResult NVFATBIN_SUCCESS \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_NULL_POINTER \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_INVALID_ARCH \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_MISSING_PTX_VERSION \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_COMPRESSION_FAILED, \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_UNRECOGNIZED_OPTION \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_COMPRESSED_SIZE_EXCEEDED \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_INTERNAL \endlink
- *
- * User is responsible for making sure all string are well-formed.
- * The size should be inclusive of the terminating null character ('\0').
- * If the final character is not '\0', one will be added automatically, but in
- * doing so, the code will be copied if it hasn't already been copied.
- */
-nvFatbinResult nvFatbinAddPTX(nvFatbinHandle handle, const char *code, size_t size, const char *arch, const char *identifier, const char *optionsCmdLine);
-
-/**
- * \ingroup creation
- * \brief   nvFatbinAddCubin adds a CUDA binary to the fatbinary.
- *
- * \param    [in] handle      nvFatbin handle.
- * \param    [in] code        The cubin.
- * \param    [in] size        The size of the cubin.
- * \param    [in] arch        The architecture that this cubin is for.
- * \param    [in] identifier  Name of the cubin, useful when extracting the fatbin with tools like cuobjdump.
- *
- * \return
- *   - \link #nvFatbinResult NVFATBIN_SUCCESS \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_INVALID_ARCH \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_ELF_ARCH_MISMATCH \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_ELF_SIZE_MISMATCH \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_COMPRESSION_FAILED, \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_UNRECOGNIZED_OPTION \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_COMPRESSED_SIZE_EXCEEDED \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_INTERNAL \endlink
- *
- * User is responsible for making sure all strings are well-formed.
- */
-nvFatbinResult nvFatbinAddCubin(nvFatbinHandle handle, const void *code, size_t size, const char *arch, const char *identifier);
-
-/**
- * \ingroup creation
- * \brief   nvFatbinAddLTOIR adds LTOIR to the fatbinary.
- *
- * \param    [in] handle      nvFatbin handle.
- * \param    [in] code        The LTOIR code.
- * \param    [in] size        The size of the LTOIR code.
- * \param    [in] arch        The architecture that this LTOIR is for.
- * \param    [in] identifier  Name of the LTOIR, useful when extracting the fatbin with tools like cuobjdump.
- * \param    [in] optionsCmdLine  Options used during JIT compilation.
- *
- * \return
- *   - \link #nvFatbinResult NVFATBIN_SUCCESS \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_NULL_POINTER \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_INVALID_ARCH \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_COMPRESSION_FAILED, \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_UNRECOGNIZED_OPTION \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_COMPRESSED_SIZE_EXCEEDED \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_INTERNAL \endlink
- *
- * User is responsible for making sure all strings are well-formed.
- */
-nvFatbinResult nvFatbinAddLTOIR(nvFatbinHandle handle, const void *code, size_t size, const char *arch, const char *identifier, const char *optionsCmdLine);
-
-/**
- * \ingroup creation
- * \brief   nvFatbinSize returns the fatbinary's size.
- *
- * \param    [in] handle      nvFatbin handle.
- * \param    [out] size       The fatbinary's size
- *
- * \return
- *   - \link #nvFatbinResult NVFATBIN_SUCCESS \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_NULL_POINTER \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_INTERNAL \endlink
- *
- */
-nvFatbinResult nvFatbinSize(nvFatbinHandle handle, size_t *size);
-
-/**
- * \ingroup creation
- * \brief   nvFatbinGet returns the completed fatbinary.
- *
- * \param    [in] handle      nvFatbin handle.
- * \param    [out] buffer     memory to store fatbinary.
- *
- * \return
- *   - \link #nvFatbinResult NVFATBIN_SUCCESS \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_NULL_POINTER \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_INTERNAL \endlink
- *
- * User is responsible for making sure the buffer is appropriately sized for the \p fatbinary.
- * You must call nvFatbinSize before using this, otherwise, it will return an error.
- * \see nvFatbinSize
- */
-nvFatbinResult nvFatbinGet(nvFatbinHandle handle, void *buffer);
-
-/**
- * \ingroup creation
- * \brief   nvFatbinVersion returns the current version of nvFatbin
- *
- * \param    [out] major        The major version.
- * \param    [out] minor        The minor version.
- * \return
- *   - \link #nvFatbinResult NVFATBIN_SUCCESS \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_NULL_POINTER \endlink
- *   - \link #nvFatbinResult NVFATBIN_ERROR_INTERNAL \endlink
- *
- */
-nvFatbinResult nvFatbinVersion(unsigned int *major, unsigned int *minor);
-#ifdef __cplusplus
-}
-#endif
-
+/*
+ * NVIDIA_COPYRIGHT_BEGIN
+ *
+ * Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
+ *
+ * NVIDIA CORPORATION and its licensors retain all intellectual property
+ * and proprietary rights in and to this software, related documentation
+ * and any modifications thereto.  Any use, reproduction, disclosure or
+ * distribution of this software and related documentation without an express
+ * license agreement from NVIDIA CORPORATION is strictly prohibited.
+ *
+ * NVIDIA_COPYRIGHT_END
+ */
+
+//
+// nvFatbin.h
+//
+
+#include <stddef.h>
+
+#ifndef nvFatbin_INCLUDED
+#define nvFatbin_INCLUDED
+
+#ifdef __cplusplus
+extern "C"
+{
+#endif
+
+/**
+ *
+ * \defgroup error Error codes
+ *
+ */
+
+/** \ingroup error
+ *
+ * \brief    The enumerated type nvFatbinResult defines API call result codes.
+ *           nvFatbin APIs return nvFatbinResult codes to indicate the result.
+ */
+
+typedef enum
+{
+  NVFATBIN_SUCCESS = 0,
+  NVFATBIN_ERROR_INTERNAL,
+  NVFATBIN_ERROR_ELF_ARCH_MISMATCH,
+  NVFATBIN_ERROR_ELF_SIZE_MISMATCH,
+  NVFATBIN_ERROR_MISSING_PTX_VERSION,
+  NVFATBIN_ERROR_NULL_POINTER,
+  NVFATBIN_ERROR_COMPRESSION_FAILED,
+  NVFATBIN_ERROR_COMPRESSED_SIZE_EXCEEDED,
+  NVFATBIN_ERROR_UNRECOGNIZED_OPTION,
+  NVFATBIN_ERROR_INVALID_ARCH,
+  NVFATBIN_ERROR_INVALID_NVVM,
+  NVFATBIN_ERROR_EMPTY_INPUT,
+} nvFatbinResult;
+
+/**
+ * \ingroup error
+ * \brief   nvFatbinGetErrorString returns an error description string for each error code.
+ *
+ * \param   [in] result       error code
+ * \return
+ *   - nullptr, if result is NVFATBIN_SUCCESS
+ *   - a string, if result is not NVFATBIN_SUCCESS
+ *
+ */
+const char *nvFatbinGetErrorString(nvFatbinResult result);
+
+/**
+ *
+ * \defgroup creation Fatbinary Creation
+ *
+ */
+
+/**
+ * \ingroup creation
+ * \brief   nvFatbinHandle is the unit of fatbin creation, and an opaque handle for
+ *          a program.
+ *
+ * To create a fatbin, an instance of nvFatbinHandle must be created first with
+ * nvFatbinCreate().
+ */
+
+typedef struct _nvFatbinHandle *nvFatbinHandle;
+
+/**
+ * \defgroup options Supported Options
+ *
+ * nvFatbin supports the options below.
+ * Option names are prefixed with a single dash (\c -).
+ * Options that take a value have an assignment operator (\c =)
+ * followed by the option value, with no spaces, e.g. \c "-host=windows".
+ *
+ * The supported options are:
+ * - \c -32 \n
+ *   Make entries 32 bit.
+ * - \c -64 \n
+ *   Make entries 64 bit.
+ * - \c -c \n
+ *   Make relocatable fatbin.
+ * - \c -compress=<bool\> \n
+ *   Enable (true) / disable (false) compression (default: true).
+ * - \c -compress-all \n
+ *   Compress everything in the fatbin, even if it's small.
+ * - \c -cuda \n
+ *   Specify CUDA (rather than OpenCL).
+ * - \c -g \n
+ *   Generate debug information.
+ * - \c -host=<name\> \n
+ *   Specify host operating system. Valid options are "linux", "windows", and "mac" (deprecated).
+ * - \c -opencl \n
+ *   Specify OpenCL (rather than CUDA).
+ */
+
+/**
+ * \ingroup creation
+ * \brief   nvFatbinCreate creates a new handle
+ *
+ * \param    [out] handle_indirect  Address of nvFatbin handle
+ * \param    [in] options       An array of strings, each containing a single option.
+ * \param    [in] optionsCount  Number of options.
+ * \return
+ *   - \link #nvFatbinResult NVFATBIN_SUCCESS \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_NULL_POINTER \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_UNRECOGNIZED_OPTION \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_INTERNAL \endlink
+ *
+ */
+nvFatbinResult nvFatbinCreate(nvFatbinHandle *handle_indirect, const char **options, size_t optionsCount);
+
+/**
+ * \ingroup creation
+ * \brief   nvFatbinDestroy destroys the handle.
+ *
+ * \param    [in] handle_indirect  Pointer to the handle.
+ * \return
+ *   - \link #nvFatbinResult NVFATBIN_SUCCESS \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_NULL_POINTER \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_INTERNAL \endlink
+ *
+ * Use of any other pointers to the handle after calling this will result in undefined behavior.
+ * The passed in handle will be set to nullptr.
+ */
+nvFatbinResult nvFatbinDestroy(nvFatbinHandle *handle_indirect);
+
+/**
+ * \ingroup creation
+ * \brief   nvFatbinAddPtx adds PTX to the fatbinary.
+ *
+ * \param    [in] handle      nvFatbin handle.
+ * \param    [in] code        The PTX code.
+ * \param    [in] size        The size of the PTX code.
+ * \param    [in] arch        The architecture that this PTX is for.
+ * \param    [in] identifier  Name of the PTX, useful when extracting the fatbin with tools like cuobjdump.
+ * \param    [in] optionsCmdLine  Options used during JIT compilation.
+ *
+ * \return
+ *   - \link #nvFatbinResult NVFATBIN_SUCCESS \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_NULL_POINTER \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_INVALID_ARCH \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_MISSING_PTX_VERSION \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_COMPRESSION_FAILED, \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_UNRECOGNIZED_OPTION \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_COMPRESSED_SIZE_EXCEEDED \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_INTERNAL \endlink
+ *
+ * User is responsible for making sure all string are well-formed.
+ * The size should be inclusive of the terminating null character ('\0').
+ * If the final character is not '\0', one will be added automatically, but in
+ * doing so, the code will be copied if it hasn't already been copied.
+ */
+nvFatbinResult nvFatbinAddPTX(nvFatbinHandle handle, const char *code, size_t size, const char *arch, const char *identifier, const char *optionsCmdLine);
+
+/**
+ * \ingroup creation
+ * \brief   nvFatbinAddCubin adds a CUDA binary to the fatbinary.
+ *
+ * \param    [in] handle      nvFatbin handle.
+ * \param    [in] code        The cubin.
+ * \param    [in] size        The size of the cubin.
+ * \param    [in] arch        The architecture that this cubin is for.
+ * \param    [in] identifier  Name of the cubin, useful when extracting the fatbin with tools like cuobjdump.
+ *
+ * \return
+ *   - \link #nvFatbinResult NVFATBIN_SUCCESS \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_INVALID_ARCH \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_ELF_ARCH_MISMATCH \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_ELF_SIZE_MISMATCH \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_COMPRESSION_FAILED, \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_UNRECOGNIZED_OPTION \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_COMPRESSED_SIZE_EXCEEDED \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_INTERNAL \endlink
+ *
+ * User is responsible for making sure all strings are well-formed.
+ */
+nvFatbinResult nvFatbinAddCubin(nvFatbinHandle handle, const void *code, size_t size, const char *arch, const char *identifier);
+
+/**
+ * \ingroup creation
+ * \brief   nvFatbinAddLTOIR adds LTOIR to the fatbinary.
+ *
+ * \param    [in] handle      nvFatbin handle.
+ * \param    [in] code        The LTOIR code.
+ * \param    [in] size        The size of the LTOIR code.
+ * \param    [in] arch        The architecture that this LTOIR is for.
+ * \param    [in] identifier  Name of the LTOIR, useful when extracting the fatbin with tools like cuobjdump.
+ * \param    [in] optionsCmdLine  Options used during JIT compilation.
+ *
+ * \return
+ *   - \link #nvFatbinResult NVFATBIN_SUCCESS \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_NULL_POINTER \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_INVALID_ARCH \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_COMPRESSION_FAILED, \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_UNRECOGNIZED_OPTION \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_COMPRESSED_SIZE_EXCEEDED \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_INTERNAL \endlink
+ *
+ * User is responsible for making sure all strings are well-formed.
+ */
+nvFatbinResult nvFatbinAddLTOIR(nvFatbinHandle handle, const void *code, size_t size, const char *arch, const char *identifier, const char *optionsCmdLine);
+
+/**
+ * \ingroup creation
+ * \brief   nvFatbinSize returns the fatbinary's size.
+ *
+ * \param    [in] handle      nvFatbin handle.
+ * \param    [out] size       The fatbinary's size
+ *
+ * \return
+ *   - \link #nvFatbinResult NVFATBIN_SUCCESS \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_NULL_POINTER \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_INTERNAL \endlink
+ *
+ */
+nvFatbinResult nvFatbinSize(nvFatbinHandle handle, size_t *size);
+
+/**
+ * \ingroup creation
+ * \brief   nvFatbinGet returns the completed fatbinary.
+ *
+ * \param    [in] handle      nvFatbin handle.
+ * \param    [out] buffer     memory to store fatbinary.
+ *
+ * \return
+ *   - \link #nvFatbinResult NVFATBIN_SUCCESS \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_NULL_POINTER \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_INTERNAL \endlink
+ *
+ * User is responsible for making sure the buffer is appropriately sized for the \p fatbinary.
+ * You must call nvFatbinSize before using this, otherwise, it will return an error.
+ * \see nvFatbinSize
+ */
+nvFatbinResult nvFatbinGet(nvFatbinHandle handle, void *buffer);
+
+/**
+ * \ingroup creation
+ * \brief   nvFatbinVersion returns the current version of nvFatbin
+ *
+ * \param    [out] major        The major version.
+ * \param    [out] minor        The minor version.
+ * \return
+ *   - \link #nvFatbinResult NVFATBIN_SUCCESS \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_NULL_POINTER \endlink
+ *   - \link #nvFatbinResult NVFATBIN_ERROR_INTERNAL \endlink
+ *
+ */
+nvFatbinResult nvFatbinVersion(unsigned int *major, unsigned int *minor);
+#ifdef __cplusplus
+}
+#endif
+
 #endif
```

## Comparing `nvidia_nvfatbin_cu12-12.4.127.dist-info/License.txt` & `nvidia_nvfatbin_cu12-12.4.99.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `nvidia_nvfatbin_cu12-12.4.127.dist-info/METADATA` & `nvidia_nvfatbin_cu12-12.4.99.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-nvfatbin-cu12
-Version: 12.4.127
+Version: 12.4.99
 Summary: NVIDIA compiler library for fatbin interaction
 Home-page: https://developer.nvidia.com/cuda-zone
 Author: Nvidia CUDA Installer Team
 Author-email: cuda_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Keywords: cuda,nvidia,runtime,machine learning,deep learning
 Classifier: Development Status :: 4 - Beta
```

## Comparing `nvidia_nvfatbin_cu12-12.4.127.dist-info/RECORD` & `nvidia_nvfatbin_cu12-12.4.99.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 nvidia/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nvidia/nvfatbin/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+nvidia/nvfatbin/bin/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+nvidia/nvfatbin/bin/nvfatbin_120_0.dll,sha256=8yxGPFGZC-cpKcWj2if2ULO7RxrWphK3AAG1qU1a9Ic,749056
 nvidia/nvfatbin/include/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-nvidia/nvfatbin/include/nvFatbin.h,sha256=6VVQaZ9WOsvBH50GNq8fl0Zt9hLGr-tjeI9OxJMcbqs,9597
-nvidia/nvfatbin/lib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-nvidia/nvfatbin/lib/libnvfatbin.so.12,sha256=nVF8K2d2DZ6EFhuL8pVpM878EfjGXfiZ3fOoir-brk8,2381192
-nvidia_nvfatbin_cu12-12.4.127.dist-info/License.txt,sha256=rW9YU_ugyg0VnQ9Y1JrkmDDC-Mk_epJki5zpCttMbM0,59262
-nvidia_nvfatbin_cu12-12.4.127.dist-info/METADATA,sha256=SA8LzXzffoyWbREQb9MpAU7WcEuFU1Xapx3JtqhcGRs,1537
-nvidia_nvfatbin_cu12-12.4.127.dist-info/WHEEL,sha256=XDTs3wIbcE-BcRO08VJlZpA6z9OaC1mOKPCGGGwuM2g,109
-nvidia_nvfatbin_cu12-12.4.127.dist-info/top_level.txt,sha256=fTkAtiFuL16nUrB9ytDDtpytz2t0B4NvYTnRzwAhO14,7
-nvidia_nvfatbin_cu12-12.4.127.dist-info/RECORD,,
+nvidia/nvfatbin/include/nvFatbin.h,sha256=B9dLF0Z2V8UVMsbq2NTVREhnbO78d4KDkzCyToQ6oZE,9868
+nvidia/nvfatbin/lib/x64/nvfatbin.lib,sha256=iGjkwLVOACe0CuOmNcc_c8xg-YcXCiljZF05ZC6tyz8,3560
+nvidia/nvfatbin/lib/x64/nvfatbin_static.lib,sha256=t2xDEglnME3GZYGevt0KLRLOvwbiFBTWyc_gnzBy3fU,4004312
+nvidia_nvfatbin_cu12-12.4.99.dist-info/License.txt,sha256=rW9YU_ugyg0VnQ9Y1JrkmDDC-Mk_epJki5zpCttMbM0,59262
+nvidia_nvfatbin_cu12-12.4.99.dist-info/METADATA,sha256=q7gvw89TdxMQPb2Y0idy85N8uM0HGuXra1zlycdd_sg,1536
+nvidia_nvfatbin_cu12-12.4.99.dist-info/WHEEL,sha256=6iYPr8vTHsyDK75jr9X0V3I9wPSVmtwr_8fdATBciGk,98
+nvidia_nvfatbin_cu12-12.4.99.dist-info/top_level.txt,sha256=fTkAtiFuL16nUrB9ytDDtpytz2t0B4NvYTnRzwAhO14,7
+nvidia_nvfatbin_cu12-12.4.99.dist-info/RECORD,,
```

