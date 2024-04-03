# Comparing `tmp/openstack-cyborg-9.0.0.tar.gz` & `tmp/openstack-cyborg-9.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstack-cyborg-9.0.0.tar", last modified: Wed Oct  5 12:11:48 2022, max compression
+gzip compressed data, was "openstack-cyborg-9.0.0.0rc1.tar", last modified: Wed Sep 14 07:50:24 2022, max compression
```

## Comparing `openstack-cyborg-9.0.0.tar` & `openstack-cyborg-9.0.0.0rc1.tar`

### file list

```diff
@@ -1,565 +1,565 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3079 2022-10-05 12:11:48.000000 openstack-cyborg-9.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      609 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23131 2022-10-05 12:11:48.000000 openstack-cyborg-9.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1853 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.667511 openstack-cyborg-9.0.0/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.683512 openstack-cyborg-9.0.0/api-ref/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3806 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/api-ref/source/arqs.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2481 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/api-ref/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2325 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/api-ref/source/deployables.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4400 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/api-ref/source/device_profile.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1940 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/api-ref/source/devices.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/api-ref/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8251 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/api-ref/source/parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.683512 openstack-cyborg-9.0.0/cyborg/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.683512 openstack-cyborg-9.0.0/cyborg/accelerator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1324 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/accelerator.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.687512 openstack-cyborg-9.0.0/cyborg/accelerator/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4333 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/common/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4029 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5837 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/configuration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.687512 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.687512 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/aichip/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/aichip/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.687512 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/aichip/huawei/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/aichip/huawei/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5120 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/aichip/huawei/ascend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1585 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5161 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fake.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.687512 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1533 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.687512 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/inspur/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/inspur/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/inspur/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5979 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/inspur/sysinfo.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.687512 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/intel/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/intel/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3195 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/intel/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10192 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/intel/sysinfo.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.687512 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/xilinx/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/xilinx/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2532 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/xilinx/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7046 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/xilinx/sysinfo.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.687512 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/gpu/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/gpu/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1709 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/gpu/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.687512 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/gpu/nvidia/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/gpu/nvidia/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/gpu/nvidia/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/gpu/nvidia/sysinfo.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6648 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/gpu/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.687512 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/modules/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/modules/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2299 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/modules/generic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.687512 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/nic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/nic/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1549 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/nic/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.691513 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/nic/intel/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/nic/intel/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1025 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/nic/intel/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8159 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/nic/intel/sysinfo.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.691513 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/qat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/qat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/qat/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.691513 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/qat/intel/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/qat/intel/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1025 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/qat/intel/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5942 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/qat/intel/sysinfo.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.691513 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.691513 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/nvmf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/nvmf/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4576 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/nvmf/nvmf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3115 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/spdk.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.691513 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/util/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/util/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6920 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/util/common_fun.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.691513 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/util/pyspdk/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/util/pyspdk/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4112 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/util/pyspdk/nvmf_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3219 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/util/pyspdk/py_spdk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4215 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/util/pyspdk/vhost_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.691513 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/vhost/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/vhost/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3505 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/vhost/vhost.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.691513 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/ssd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/ssd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2046 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/ssd/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.691513 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/ssd/inspur/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/ssd/inspur/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/ssd/inspur/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/ssd/inspur/sysinfo.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6404 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/accelerator/drivers/ssd/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.691513 openstack-cyborg-9.0.0/cyborg/agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/agent/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2998 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/agent/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2741 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/agent/resource_tracker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2043 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/agent/rpcapi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.695513 openstack-cyborg-9.0.0/cyborg/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2237 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1308 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.695513 openstack-cyborg-9.0.0/cyborg/api/controllers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/controllers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4806 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/controllers/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1993 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/controllers/link.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3587 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/controllers/root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6387 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/controllers/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1273 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/controllers/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.695513 openstack-cyborg-9.0.0/cyborg/api/controllers/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4951 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/controllers/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14453 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/controllers/v2/arqs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6907 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/controllers/v2/deployables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13186 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/controllers/v2/device_profiles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4290 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/controllers/v2/devices.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      834 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/controllers/v2/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1929 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/controllers/v2/versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/expose.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3298 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/hooks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.695513 openstack-cyborg-9.0.0/cyborg/api/middleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      931 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/middleware/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2616 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/middleware/auth_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2742 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/middleware/parsable_error.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/rest_api_version_history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1234 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/api/wsgi_app.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.695513 openstack-cyborg-9.0.0/cyborg/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1280 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/cmd/agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1158 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/cmd/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/cmd/conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2826 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/cmd/dbsync.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2704 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/cmd/status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.699513 openstack-cyborg-9.0.0/cyborg/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8327 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/common/authorize_wsgi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3055 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12099 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/common/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/common/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4136 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/common/nova_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1448 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/common/paths.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15050 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/common/placement_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3115 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/common/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3872 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/common/rpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4664 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/common/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17847 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/common/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.699513 openstack-cyborg-9.0.0/cyborg/conductor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conductor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1566 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conductor/handlers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21510 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conductor/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4582 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conductor/rpcapi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.699513 openstack-cyborg-9.0.0/cyborg/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1291 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conf/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1338 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conf/agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2760 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conf/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conf/database.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3211 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conf/default.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3460 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conf/devices.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5101 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conf/glance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1259 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conf/keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1452 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conf/nova.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2168 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conf/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1538 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conf/placement.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1882 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conf/service_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3992 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/conf/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8460 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.703513 openstack-cyborg-9.0.0/cyborg/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8356 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1473 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/migration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.703513 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.703513 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1984 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.703513 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/22fb1af2d51e_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/4cc1d79978fc_add_ssd_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/57539722e5cf_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/589ff20545b7_add_aichip_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/60d8ac91fd20_add_description_field_to_dps.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/62bcf2610c5d_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/7a4fd0fc3f8c_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/7b696fd94949_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/7e6f1f107f2b_add_qat_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/899cead40bc9_add_nic_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3347 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/c1b5abada09c_update_for_nova_integ.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2973 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/d6f033d8fa5b_add_quota_related_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7850 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/ede4e3f1a232_new_db_schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4393 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/f50980397351_initial_migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      975 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44090 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3385 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10300 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/models.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.703513 openstack-cyborg-9.0.0/cyborg/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6716 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/hacking/checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.703513 openstack-cyborg-9.0.0/cyborg/image/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/image/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3540 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/image/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24835 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/image/glance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.707514 openstack-cyborg-9.0.0/cyborg/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2714 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/arq.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4736 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/attach_handle.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3639 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/attribute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8142 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4360 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/control_path.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6900 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/deployable.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3872 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/device.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5079 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/device_profile.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.707514 openstack-cyborg-9.0.0/cyborg/objects/driver_objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/driver_objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3029 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/driver_objects/driver_attach_handle.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2630 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/driver_objects/driver_attribute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2445 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/driver_objects/driver_controlpath_id.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5621 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/driver_objects/driver_deployable.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7119 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/driver_objects/driver_device.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14050 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/ext_arq.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.707514 openstack-cyborg-9.0.0/cyborg/objects/extarq/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/extarq/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10675 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/extarq/ext_arq_job.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10217 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/extarq/fpga_ext_arq.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/objects/fields.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.707514 openstack-cyborg-9.0.0/cyborg/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1168 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7458 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/policies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4602 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/policies/device_profiles.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.707514 openstack-cyborg-9.0.0/cyborg/privsep/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1222 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/privsep/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7823 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1879 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/service_auth.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.707514 openstack-cyborg-9.0.0/cyborg/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6503 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.707514 openstack-cyborg-9.0.0/cyborg/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4227 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/post_mortem_debug.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.711514 openstack-cyborg-9.0.0/cyborg/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1349 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.711514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.711514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.711514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/aichip/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/aichip/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.711514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/aichip/huawei/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/aichip/huawei/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2166 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/aichip/huawei/test_ascend.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.711514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.711514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/inspur/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/inspur/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5761 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/inspur/test_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.711514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/intel/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/intel/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10729 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/intel/prepare_test_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5820 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/intel/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/test_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.711514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/xilinx/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/xilinx/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5675 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/xilinx/test_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.711514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/gpu/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/gpu/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.715514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/gpu/nvidia/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/gpu/nvidia/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/gpu/nvidia/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/gpu/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4990 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/gpu/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.715514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/nic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/nic/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.715514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/nic/intel/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/nic/intel/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9216 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/nic/intel/prepare_test_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5679 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/nic/intel/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1122 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/nic/test_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.715514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/qat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/qat/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.715514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/qat/intel/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/qat/intel/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9848 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/qat/intel/prepare_test_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4580 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/qat/intel/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/qat/test_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.715514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/spdk/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/spdk/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.715514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/spdk/nvmf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/spdk/nvmf/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4732 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/spdk/nvmf/test_nvmf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.715514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/spdk/vhost/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/spdk/vhost/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5325 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/spdk/vhost/test_vhost.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.715514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/ssd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/ssd/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.715514 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/ssd/inspur/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/ssd/inspur/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1276 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/ssd/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5861 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/ssd/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5378 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/test_fake_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.715514 openstack-cyborg-9.0.0/cyborg/tests/unit/agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/agent/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2490 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/agent/test_resource_tracker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2136 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/agent/test_rpcapi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.715514 openstack-cyborg-9.0.0/cyborg/tests/unit/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9667 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/api/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.715514 openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.719514 openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1230 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16781 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/test_arqs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4220 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/test_deployables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12561 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/test_device_profiles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5039 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/test_devices.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6771 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/test_fpga_program.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4328 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/test_microversion.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.719514 openstack-cyborg-9.0.0/cyborg/tests/unit/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3479 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/cmd/test_status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.719514 openstack-cyborg-9.0.0/cyborg/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5051 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/common/test_nova_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.719514 openstack-cyborg-9.0.0/cyborg/tests/unit/conductor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/conductor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6782 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/conductor/test_manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.719514 openstack-cyborg-9.0.0/cyborg/tests/unit/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2120 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/db/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4935 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_db_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5384 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_db_attach_handle.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1351 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_db_attribute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1103 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_db_control_path.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4527 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_db_deployable.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4376 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_db_device.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6500 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_db_device_profile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2835 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_db_extarq.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6163 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_migrations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7800 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/db/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2338 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/fake_attach_handle.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1699 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/fake_attribute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1879 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/fake_deployable.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2406 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/fake_device.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3854 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/fake_device_profile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5748 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/fake_driver_device.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12567 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/fake_extarq.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2400 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/fake_physical_function.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2387 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/fake_virtual_function.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.719514 openstack-cyborg-9.0.0/cyborg/tests/unit/image/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/image/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/image/test_glance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.723515 openstack-cyborg-9.0.0/cyborg/tests/unit/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8536 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_attach_handle.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5361 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_control_path.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5801 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_deployable.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7239 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_device.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6114 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_device_profile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17382 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_ext_arq_job.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23304 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_extarq.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18192 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_fpga_ext_arq.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7302 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_objects.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.723515 openstack-cyborg-9.0.0/cyborg/tests/unit/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3572 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/policies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7366 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/policies/test_device_profiles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1733 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/policy_fixture.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.723515 openstack-cyborg-9.0.0/cyborg/tests/unit/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5966 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/services/_test_placement_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1560 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10215 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/tests/unit/test_hacking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1466 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/cyborg.conf.intelnic.sample
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.723515 openstack-cyborg-9.0.0/devstack/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.723515 openstack-cyborg-9.0.0/devstack/lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9212 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/devstack/lib/cyborg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1819 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.723515 openstack-cyborg-9.0.0/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.675511 openstack-cyborg-9.0.0/doc/api_samples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.723515 openstack-cyborg-9.0.0/doc/api_samples/accelerator_requests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      712 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/accelerator_requests/accelerator_requests-after-update-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/accelerator_requests/accelerator_requests-before-update-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      661 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/accelerator_requests/accelerator_requests-create-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/accelerator_requests/accelerator_requests-getone-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1500 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/accelerator_requests/accelerator_requests-list-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/accelerator_requests/accelerator_requests-patch-curl.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/accelerator_requests/accelerator_requests-post-curl.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.723515 openstack-cyborg-9.0.0/doc/api_samples/deployables/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      758 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/deployables/deployables-getone-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/deployables/deployables-list-resp.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.723515 openstack-cyborg-9.0.0/doc/api_samples/device_profiles/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/device_profiles/device_profiles-create-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      597 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/device_profiles/device_profiles-getone-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/device_profiles/device_profiles-list-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      542 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/device_profiles/device_profiles-post-curl-with-bitstream.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/device_profiles/device_profiles-post-curl.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.723515 openstack-cyborg-9.0.0/doc/api_samples/device_profiles/v22/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      597 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/device_profiles/v22/device_profiles-getone-resp.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.727515 openstack-cyborg-9.0.0/doc/api_samples/devices/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/devices/devices-getone-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/api_samples/devices/devices-list-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.727515 openstack-cyborg-9.0.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.727515 openstack-cyborg-9.0.0/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/admin/config-wsgi.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9254 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/admin/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.727515 openstack-cyborg-9.0.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/cli/cyborg-status.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/cli/index.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4238 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.727515 openstack-cyborg-9.0.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/configuration/config-options.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/configuration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11599 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/configuration/policy-concepts.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1478 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/configuration/policy-guide.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/configuration/policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/configuration/sample-config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1198 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/configuration/sample-policy.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.727515 openstack-cyborg-9.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3599 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4480 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/contributor/devstack_setup.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/contributor/driver-development-guide.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12804 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/contributor/microversions.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2632 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/contributor/releasenotes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/contributor/rest_api_version_history.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.731516 openstack-cyborg-9.0.0/doc/source/figures/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    39362 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/figures/cyborg-architecture.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9730 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/figures/cyborg-nova-interaction-workflow.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37829 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/figures/cyborg-nova-interaction.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2438 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.731516 openstack-cyborg-9.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5835 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/install/common.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/install/install-from-pip.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/install/install-from-source.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.731516 openstack-cyborg-9.0.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2420 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/reference/driver-table.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1923 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/reference/support-matrix.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.731516 openstack-cyborg-9.0.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/user/architecture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1330 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/user/introduction.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/doc/source/user/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.679512 openstack-cyborg-9.0.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.731516 openstack-cyborg-9.0.0/etc/cyborg/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/etc/cyborg/README.cyborg.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/etc/cyborg/README.policy.yaml.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/etc/cyborg/api-paste.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/etc/cyborg/policy.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.731516 openstack-cyborg-9.0.0/openstack_cyborg.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1853 2022-10-05 12:11:48.000000 openstack-cyborg-9.0.0/openstack_cyborg.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18120 2022-10-05 12:11:48.000000 openstack-cyborg-9.0.0/openstack_cyborg.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-10-05 12:11:48.000000 openstack-cyborg-9.0.0/openstack_cyborg.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2022-10-05 12:11:48.000000 openstack-cyborg-9.0.0/openstack_cyborg.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-10-05 12:11:48.000000 openstack-cyborg-9.0.0/openstack_cyborg.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-10-05 12:11:48.000000 openstack-cyborg-9.0.0/openstack_cyborg.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2022-10-05 12:11:48.000000 openstack-cyborg-9.0.0/openstack_cyborg.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2022-10-05 12:11:48.000000 openstack-cyborg-9.0.0/openstack_cyborg.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.679512 openstack-cyborg-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.735516 openstack-cyborg-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/add-programming-method-051b9c4244c35c71.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/add-project_id-to-arq-patch-api-8270cbb26c68af46.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/add-xilinx-fpga-driver-1c98c6a95d8e1f9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/add_ARQ_UNBIND_FAILED_status-ea8636c64dd616eb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/add_description_to_device_profile-3c2efcbd54dac7b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/basic-framework-28d6b42d9bf684af.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/bug-1928174-delete_trait_from_placement-266caf73cf289759.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/configure-multiple-vgpu-types-a60d09dfb5b7be4b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/cyborg-nova-interaction-8fe4e49e3c9b3b7b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/cyborg-status-upgrade-check-framework-567f8df30b971f13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/drop-py-3-6-and-3-7--37951d4a79dffdbd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/drop-python2-support-in-ussuri-e64f79db4e88ca19.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/fpga-driver-8b1635e92b1297c1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/generic-driver-88427acd7c7c12df.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/implement_oslo_privsep-4fc6e15360c92772.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/inspur-fpga-driver-0257d2aeda9537fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/inspur-nvme-ssd-faeddc0b09250acc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/intel-nic-driver-f93adad86a23ceb9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/intel-qat-driver-a7b4c8f110d41e0b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/introduce-bandit-security-linter-339d3f12b6200d64.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/introduce-microversion-39c7f5cc6af4a139.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/policy-file-default-value-change-de14a3688357b081.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3125 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/policy_refresh_base_and_device_profile-cef00fca580d2323.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/remove-OPAE-dependency-from-devstack-f6db83bb37761340.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/removed-download-modules-540fa0607d7df967.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/show-device-profile-with-name-27bf5a301a631c04.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/notes/spdk-driver-89b178e1a2db29c0.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5123 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/setup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/setup/deploy-cyborg.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.679512 openstack-cyborg-9.0.0/setup/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.679512 openstack-cyborg-9.0.0/setup/roles/deploy_agent/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/setup/roles/deploy_agent/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/setup/roles/deploy_agent/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/setup/roles/deploy_agent/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/setup/roles/deploy_agent/templates/openstack-cyborg-agent.service.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.679512 openstack-cyborg-9.0.0/setup/roles/deploy_api/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/setup/roles/deploy_api/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/setup/roles/deploy_api/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/setup/roles/deploy_api/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/setup/roles/deploy_api/templates/openstack-cyborg-api.service.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.679512 openstack-cyborg-9.0.0/setup/roles/deploy_conductor/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/setup/roles/deploy_conductor/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/setup/roles/deploy_conductor/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/setup/roles/deploy_conductor/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/setup/roles/deploy_conductor/templates/openstack-cyborg-conductor.service.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.679512 openstack-cyborg-9.0.0/setup/roles/generate_credentials/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/setup/roles/generate_credentials/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/setup/roles/generate_credentials/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.679512 openstack-cyborg-9.0.0/setup/roles/install_package/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/setup/roles/install_package/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/setup/roles/install_package/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.679512 openstack-cyborg-9.0.0/setup/roles/template_config/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/setup/roles/template_config/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/setup/roles/template_config/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/setup/roles/template_config/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/setup/roles/template_config/templates/cyborg.conf.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.679512 openstack-cyborg-9.0.0/setup/roles/validate_agent/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/setup/roles/validate_agent/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/setup/roles/validate_agent/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.679512 openstack-cyborg-9.0.0/setup/roles/validate_api/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/setup/roles/validate_api/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/setup/roles/validate_api/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.679512 openstack-cyborg-9.0.0/setup/roles/validate_conductor/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/setup/roles/validate_conductor/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/setup/roles/validate_conductor/tasks/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2232 2022-10-05 12:11:48.743516 openstack-cyborg-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1560 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/tools/check-cherry-picks.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-05 12:11:48.739516 openstack-cyborg-9.0.0/tools/config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/tools/config/cyborg-config-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/tools/config/cyborg-policy-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/tools/flake8wrap.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4657 2022-10-05 12:10:09.000000 openstack-cyborg-9.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.616503 openstack-cyborg-9.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3079 2022-09-14 07:50:23.000000 openstack-cyborg-9.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      609 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23141 2022-09-14 07:50:23.000000 openstack-cyborg-9.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1858 2022-09-14 07:50:24.616503 openstack-cyborg-9.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.544503 openstack-cyborg-9.0.0.0rc1/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.564503 openstack-cyborg-9.0.0.0rc1/api-ref/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3806 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/api-ref/source/arqs.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2481 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2325 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/api-ref/source/deployables.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4400 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/api-ref/source/device_profile.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1940 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/api-ref/source/devices.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/api-ref/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8251 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/api-ref/source/parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.564503 openstack-cyborg-9.0.0.0rc1/cyborg/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.564503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1324 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/accelerator.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.564503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4333 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/common/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4029 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5837 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/configuration.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.564503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.564503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/aichip/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/aichip/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.564503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/aichip/huawei/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/aichip/huawei/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5120 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/aichip/huawei/ascend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1585 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5161 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fake.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.564503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1533 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.564503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/inspur/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/inspur/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/inspur/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5979 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/inspur/sysinfo.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.568503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/intel/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/intel/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3195 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/intel/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10192 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/intel/sysinfo.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.568503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/xilinx/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/xilinx/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2532 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/xilinx/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7046 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/xilinx/sysinfo.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.568503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/gpu/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/gpu/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1709 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/gpu/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.568503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/gpu/nvidia/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/gpu/nvidia/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/gpu/nvidia/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/gpu/nvidia/sysinfo.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6648 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/gpu/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.568503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/modules/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/modules/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2299 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/modules/generic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.568503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/nic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/nic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1549 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/nic/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.568503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/nic/intel/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/nic/intel/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1025 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/nic/intel/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8159 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/nic/intel/sysinfo.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.568503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/qat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/qat/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/qat/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.568503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/qat/intel/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/qat/intel/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1025 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/qat/intel/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5942 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/qat/intel/sysinfo.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.568503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.568503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/nvmf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/nvmf/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4576 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/nvmf/nvmf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3115 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/spdk.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.568503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/util/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/util/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6920 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/util/common_fun.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.572503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/util/pyspdk/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/util/pyspdk/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4112 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/util/pyspdk/nvmf_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3219 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/util/pyspdk/py_spdk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4215 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/util/pyspdk/vhost_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.572503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/vhost/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/vhost/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3505 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/vhost/vhost.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.572503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/ssd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/ssd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2046 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/ssd/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.572503 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/ssd/inspur/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/ssd/inspur/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/ssd/inspur/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/ssd/inspur/sysinfo.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6404 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/ssd/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.572503 openstack-cyborg-9.0.0.0rc1/cyborg/agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/agent/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2998 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/agent/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2741 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/agent/resource_tracker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2043 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/agent/rpcapi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.572503 openstack-cyborg-9.0.0.0rc1/cyborg/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2237 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1308 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.572503 openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4806 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1993 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/link.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3587 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6387 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1273 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.576503 openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4951 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14453 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/v2/arqs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6907 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/v2/deployables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13186 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/v2/device_profiles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4290 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/v2/devices.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      834 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/v2/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1929 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/v2/versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/expose.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3298 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/hooks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.576503 openstack-cyborg-9.0.0.0rc1/cyborg/api/middleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      931 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/middleware/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2616 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/middleware/auth_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2742 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/middleware/parsable_error.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/rest_api_version_history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1234 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/api/wsgi_app.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.576503 openstack-cyborg-9.0.0.0rc1/cyborg/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1280 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/cmd/agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1158 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/cmd/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/cmd/conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2826 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/cmd/dbsync.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2704 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/cmd/status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.576503 openstack-cyborg-9.0.0.0rc1/cyborg/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8327 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/common/authorize_wsgi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3055 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12099 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/common/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/common/i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4136 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/common/nova_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1448 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/common/paths.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15050 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/common/placement_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3115 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/common/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3872 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/common/rpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4664 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/common/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17847 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/common/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.576503 openstack-cyborg-9.0.0.0rc1/cyborg/conductor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conductor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1566 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conductor/handlers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21510 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conductor/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4582 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conductor/rpcapi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.580503 openstack-cyborg-9.0.0.0rc1/cyborg/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1291 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conf/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1338 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conf/agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2760 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conf/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conf/database.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3211 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conf/default.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3460 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conf/devices.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5101 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conf/glance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1259 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conf/keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1452 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conf/nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2168 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conf/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1538 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conf/placement.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1882 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conf/service_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3992 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/conf/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8460 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/context.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.580503 openstack-cyborg-9.0.0.0rc1/cyborg/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8356 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1473 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/migration.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.580503 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.580503 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1984 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.584503 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/22fb1af2d51e_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/4cc1d79978fc_add_ssd_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/57539722e5cf_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/589ff20545b7_add_aichip_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/60d8ac91fd20_add_description_field_to_dps.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/62bcf2610c5d_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/7a4fd0fc3f8c_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/7b696fd94949_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/7e6f1f107f2b_add_qat_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/899cead40bc9_add_nic_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3347 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/c1b5abada09c_update_for_nova_integ.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2973 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/d6f033d8fa5b_add_quota_related_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7850 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/ede4e3f1a232_new_db_schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4393 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/f50980397351_initial_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      975 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44090 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3385 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10300 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/models.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.584503 openstack-cyborg-9.0.0.0rc1/cyborg/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6716 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/hacking/checks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.584503 openstack-cyborg-9.0.0.0rc1/cyborg/image/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/image/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3540 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/image/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24835 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/image/glance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.584503 openstack-cyborg-9.0.0.0rc1/cyborg/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2714 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/arq.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4736 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/attach_handle.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3639 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/attribute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8142 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4360 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/control_path.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6900 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/deployable.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3872 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/device.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5079 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/device_profile.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.584503 openstack-cyborg-9.0.0.0rc1/cyborg/objects/driver_objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/driver_objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3029 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/driver_objects/driver_attach_handle.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2630 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/driver_objects/driver_attribute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2445 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/driver_objects/driver_controlpath_id.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5621 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/driver_objects/driver_deployable.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7119 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/driver_objects/driver_device.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14050 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/ext_arq.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.584503 openstack-cyborg-9.0.0.0rc1/cyborg/objects/extarq/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/extarq/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10675 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/extarq/ext_arq_job.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10217 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/extarq/fpga_ext_arq.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/objects/fields.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.588503 openstack-cyborg-9.0.0.0rc1/cyborg/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1168 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7458 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4602 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/policies/device_profiles.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.588503 openstack-cyborg-9.0.0.0rc1/cyborg/privsep/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1222 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/privsep/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7823 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1879 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/service_auth.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.588503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6503 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.588503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4227 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/post_mortem_debug.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.588503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1349 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.588503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.588503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.588503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/aichip/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/aichip/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.588503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/aichip/huawei/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/aichip/huawei/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2166 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/aichip/huawei/test_ascend.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.588503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.588503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/inspur/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/inspur/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5761 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/inspur/test_driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.592503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/intel/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/intel/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10729 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/intel/prepare_test_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5820 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/intel/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/test_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.592503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/xilinx/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/xilinx/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5675 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/xilinx/test_driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.592503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/gpu/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/gpu/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.592503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/gpu/nvidia/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/gpu/nvidia/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/gpu/nvidia/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/gpu/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4990 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/gpu/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.592503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/nic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/nic/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.592503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/nic/intel/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/nic/intel/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9216 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/nic/intel/prepare_test_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5679 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/nic/intel/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1122 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/nic/test_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.592503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/qat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/qat/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.592503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/qat/intel/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/qat/intel/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9848 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/qat/intel/prepare_test_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4580 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/qat/intel/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/qat/test_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.592503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/spdk/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/spdk/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.592503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/spdk/nvmf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/spdk/nvmf/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4732 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/spdk/nvmf/test_nvmf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.592503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/spdk/vhost/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/spdk/vhost/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5325 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/spdk/vhost/test_vhost.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.592503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/ssd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/ssd/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.592503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/ssd/inspur/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/ssd/inspur/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1276 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/ssd/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5861 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/ssd/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5378 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/test_fake_driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.592503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/agent/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2490 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/agent/test_resource_tracker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2136 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/agent/test_rpcapi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.596503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9667 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.596503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.596503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1230 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16781 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/test_arqs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4220 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/test_deployables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12561 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/test_device_profiles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5039 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/test_devices.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6771 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/test_fpga_program.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4328 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/test_microversion.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.596503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3479 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/cmd/test_status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.596503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5051 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/common/test_nova_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.596503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/conductor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/conductor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6782 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/conductor/test_manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.596503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2120 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4935 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_db_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5384 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_db_attach_handle.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1351 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_db_attribute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1103 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_db_control_path.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4527 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_db_deployable.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4376 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_db_device.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6500 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_db_device_profile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2835 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_db_extarq.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6163 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_migrations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7800 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2338 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_attach_handle.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1699 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_attribute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1879 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_deployable.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2406 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_device.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3854 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_device_profile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5748 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_driver_device.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12567 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_extarq.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2400 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_physical_function.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2387 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_virtual_function.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.600503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/image/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/image/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/image/test_glance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.600503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8536 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_attach_handle.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5361 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_control_path.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5801 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_deployable.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7239 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_device.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6114 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_device_profile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17382 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_ext_arq_job.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23304 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_extarq.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18192 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_fpga_ext_arq.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7302 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_objects.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.600503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3572 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7366 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/policies/test_device_profiles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1733 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/policy_fixture.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.600503 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5966 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/services/_test_placement_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1560 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10215 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/test_hacking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1466 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/cyborg.conf.intelnic.sample
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.600503 openstack-cyborg-9.0.0.0rc1/devstack/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.600503 openstack-cyborg-9.0.0.0rc1/devstack/lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9212 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/devstack/lib/cyborg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1819 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.600503 openstack-cyborg-9.0.0.0rc1/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.556503 openstack-cyborg-9.0.0.0rc1/doc/api_samples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.600503 openstack-cyborg-9.0.0.0rc1/doc/api_samples/accelerator_requests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      712 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/accelerator_requests/accelerator_requests-after-update-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/accelerator_requests/accelerator_requests-before-update-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      661 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/accelerator_requests/accelerator_requests-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/accelerator_requests/accelerator_requests-getone-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1500 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/accelerator_requests/accelerator_requests-list-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/accelerator_requests/accelerator_requests-patch-curl.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/accelerator_requests/accelerator_requests-post-curl.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.600503 openstack-cyborg-9.0.0.0rc1/doc/api_samples/deployables/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      758 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/deployables/deployables-getone-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/deployables/deployables-list-resp.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.604503 openstack-cyborg-9.0.0.0rc1/doc/api_samples/device_profiles/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/device_profiles/device_profiles-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      597 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/device_profiles/device_profiles-getone-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/device_profiles/device_profiles-list-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      542 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/device_profiles/device_profiles-post-curl-with-bitstream.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/device_profiles/device_profiles-post-curl.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.604503 openstack-cyborg-9.0.0.0rc1/doc/api_samples/device_profiles/v22/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      597 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/device_profiles/v22/device_profiles-getone-resp.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.604503 openstack-cyborg-9.0.0.0rc1/doc/api_samples/devices/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/devices/devices-getone-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/api_samples/devices/devices-list-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.604503 openstack-cyborg-9.0.0.0rc1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.604503 openstack-cyborg-9.0.0.0rc1/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/admin/config-wsgi.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9254 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/admin/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.604503 openstack-cyborg-9.0.0.0rc1/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/cli/cyborg-status.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/cli/index.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4238 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.604503 openstack-cyborg-9.0.0.0rc1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/configuration/config-options.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11599 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/configuration/policy-concepts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1478 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/configuration/policy-guide.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/configuration/policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/configuration/sample-config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1198 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/configuration/sample-policy.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.604503 openstack-cyborg-9.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3599 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4480 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/contributor/devstack_setup.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/contributor/driver-development-guide.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12804 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/contributor/microversions.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2632 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/contributor/releasenotes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/contributor/rest_api_version_history.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.604503 openstack-cyborg-9.0.0.0rc1/doc/source/figures/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    39362 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/figures/cyborg-architecture.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9730 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/figures/cyborg-nova-interaction-workflow.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37829 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/figures/cyborg-nova-interaction.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2438 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.608502 openstack-cyborg-9.0.0.0rc1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5835 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/install/common.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/install/install-from-pip.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/install/install-from-source.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.608502 openstack-cyborg-9.0.0.0rc1/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2420 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/reference/driver-table.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1923 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/reference/support-matrix.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.608502 openstack-cyborg-9.0.0.0rc1/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/user/architecture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1330 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/user/introduction.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/doc/source/user/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.556503 openstack-cyborg-9.0.0.0rc1/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.608502 openstack-cyborg-9.0.0.0rc1/etc/cyborg/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/etc/cyborg/README.cyborg.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/etc/cyborg/README.policy.yaml.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/etc/cyborg/api-paste.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/etc/cyborg/policy.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.608502 openstack-cyborg-9.0.0.0rc1/openstack_cyborg.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1858 2022-09-14 07:50:23.000000 openstack-cyborg-9.0.0.0rc1/openstack_cyborg.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18120 2022-09-14 07:50:24.000000 openstack-cyborg-9.0.0.0rc1/openstack_cyborg.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-09-14 07:50:23.000000 openstack-cyborg-9.0.0.0rc1/openstack_cyborg.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2022-09-14 07:50:23.000000 openstack-cyborg-9.0.0.0rc1/openstack_cyborg.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-09-14 07:50:23.000000 openstack-cyborg-9.0.0.0rc1/openstack_cyborg.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-09-14 07:50:23.000000 openstack-cyborg-9.0.0.0rc1/openstack_cyborg.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2022-09-14 07:50:23.000000 openstack-cyborg-9.0.0.0rc1/openstack_cyborg.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2022-09-14 07:50:23.000000 openstack-cyborg-9.0.0.0rc1/openstack_cyborg.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.556503 openstack-cyborg-9.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.612502 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/add-programming-method-051b9c4244c35c71.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/add-project_id-to-arq-patch-api-8270cbb26c68af46.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/add-xilinx-fpga-driver-1c98c6a95d8e1f9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/add_ARQ_UNBIND_FAILED_status-ea8636c64dd616eb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/add_description_to_device_profile-3c2efcbd54dac7b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/basic-framework-28d6b42d9bf684af.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/bug-1928174-delete_trait_from_placement-266caf73cf289759.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/configure-multiple-vgpu-types-a60d09dfb5b7be4b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/cyborg-nova-interaction-8fe4e49e3c9b3b7b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/cyborg-status-upgrade-check-framework-567f8df30b971f13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/drop-py-3-6-and-3-7--37951d4a79dffdbd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/drop-python2-support-in-ussuri-e64f79db4e88ca19.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/fpga-driver-8b1635e92b1297c1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/generic-driver-88427acd7c7c12df.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/implement_oslo_privsep-4fc6e15360c92772.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/inspur-fpga-driver-0257d2aeda9537fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/inspur-nvme-ssd-faeddc0b09250acc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/intel-nic-driver-f93adad86a23ceb9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/intel-qat-driver-a7b4c8f110d41e0b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/introduce-bandit-security-linter-339d3f12b6200d64.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/introduce-microversion-39c7f5cc6af4a139.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/policy-file-default-value-change-de14a3688357b081.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3125 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/policy_refresh_base_and_device_profile-cef00fca580d2323.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/remove-OPAE-dependency-from-devstack-f6db83bb37761340.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/removed-download-modules-540fa0607d7df967.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/show-device-profile-with-name-27bf5a301a631c04.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/notes/spdk-driver-89b178e1a2db29c0.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.612502 openstack-cyborg-9.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5123 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.612502 openstack-cyborg-9.0.0.0rc1/setup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/setup/deploy-cyborg.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.560503 openstack-cyborg-9.0.0.0rc1/setup/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.560503 openstack-cyborg-9.0.0.0rc1/setup/roles/deploy_agent/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.612502 openstack-cyborg-9.0.0.0rc1/setup/roles/deploy_agent/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/setup/roles/deploy_agent/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.612502 openstack-cyborg-9.0.0.0rc1/setup/roles/deploy_agent/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/setup/roles/deploy_agent/templates/openstack-cyborg-agent.service.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.560503 openstack-cyborg-9.0.0.0rc1/setup/roles/deploy_api/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.612502 openstack-cyborg-9.0.0.0rc1/setup/roles/deploy_api/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/setup/roles/deploy_api/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.612502 openstack-cyborg-9.0.0.0rc1/setup/roles/deploy_api/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/setup/roles/deploy_api/templates/openstack-cyborg-api.service.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.560503 openstack-cyborg-9.0.0.0rc1/setup/roles/deploy_conductor/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.612502 openstack-cyborg-9.0.0.0rc1/setup/roles/deploy_conductor/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/setup/roles/deploy_conductor/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.612502 openstack-cyborg-9.0.0.0rc1/setup/roles/deploy_conductor/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/setup/roles/deploy_conductor/templates/openstack-cyborg-conductor.service.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.560503 openstack-cyborg-9.0.0.0rc1/setup/roles/generate_credentials/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.616503 openstack-cyborg-9.0.0.0rc1/setup/roles/generate_credentials/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/setup/roles/generate_credentials/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.560503 openstack-cyborg-9.0.0.0rc1/setup/roles/install_package/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.616503 openstack-cyborg-9.0.0.0rc1/setup/roles/install_package/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/setup/roles/install_package/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.560503 openstack-cyborg-9.0.0.0rc1/setup/roles/template_config/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.616503 openstack-cyborg-9.0.0.0rc1/setup/roles/template_config/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/setup/roles/template_config/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.616503 openstack-cyborg-9.0.0.0rc1/setup/roles/template_config/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/setup/roles/template_config/templates/cyborg.conf.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.560503 openstack-cyborg-9.0.0.0rc1/setup/roles/validate_agent/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.616503 openstack-cyborg-9.0.0.0rc1/setup/roles/validate_agent/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/setup/roles/validate_agent/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.560503 openstack-cyborg-9.0.0.0rc1/setup/roles/validate_api/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.616503 openstack-cyborg-9.0.0.0rc1/setup/roles/validate_api/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/setup/roles/validate_api/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.560503 openstack-cyborg-9.0.0.0rc1/setup/roles/validate_conductor/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.616503 openstack-cyborg-9.0.0.0rc1/setup/roles/validate_conductor/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/setup/roles/validate_conductor/tasks/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2232 2022-09-14 07:50:24.616503 openstack-cyborg-9.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.616503 openstack-cyborg-9.0.0.0rc1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1560 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/tools/check-cherry-picks.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-14 07:50:24.616503 openstack-cyborg-9.0.0.0rc1/tools/config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/tools/config/cyborg-config-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/tools/config/cyborg-policy-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/tools/flake8wrap.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4657 2022-09-14 07:48:36.000000 openstack-cyborg-9.0.0.0rc1/tox.ini
```

### Comparing `openstack-cyborg-9.0.0/.zuul.yaml` & `openstack-cyborg-9.0.0.0rc1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/AUTHORS` & `openstack-cyborg-9.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/CONTRIBUTING.rst` & `openstack-cyborg-9.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/ChangeLog` & `openstack-cyborg-9.0.0.0rc1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0
------
+9.0.0.0rc1
+----------
 
 * Fix the compatible issue
 * Get return None for default
 * Add extra driver comment for default opt
 * fix doc comment
 * Add Xilinx FPGA driver in doc
 * Fix code and comment to reasonable
```

### Comparing `openstack-cyborg-9.0.0/HACKING.rst` & `openstack-cyborg-9.0.0.0rc1/HACKING.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/LICENSE` & `openstack-cyborg-9.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/PKG-INFO` & `openstack-cyborg-9.0.0.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: openstack-cyborg
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Distributed Acceleration Management as a Service
 Home-page: https://docs.openstack.org/cyborg/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ======
         Cyborg
```

### Comparing `openstack-cyborg-9.0.0/README.rst` & `openstack-cyborg-9.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/api-ref/source/arqs.inc` & `openstack-cyborg-9.0.0.0rc1/api-ref/source/arqs.inc`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/api-ref/source/conf.py` & `openstack-cyborg-9.0.0.0rc1/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/api-ref/source/deployables.inc` & `openstack-cyborg-9.0.0.0rc1/api-ref/source/deployables.inc`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/api-ref/source/device_profile.inc` & `openstack-cyborg-9.0.0.0rc1/api-ref/source/device_profile.inc`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/api-ref/source/devices.inc` & `openstack-cyborg-9.0.0.0rc1/api-ref/source/devices.inc`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/api-ref/source/parameters.yaml` & `openstack-cyborg-9.0.0.0rc1/api-ref/source/parameters.yaml`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/bindep.txt` & `openstack-cyborg-9.0.0.0rc1/bindep.txt`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/__init__.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/__init__.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/__init__.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/__init__.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/accelerator.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/accelerator.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/common/exception.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/common/exception.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/common/utils.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/common/utils.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/configuration.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/configuration.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/aichip/huawei/ascend.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/aichip/huawei/ascend.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/driver.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/driver.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fake.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fake.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/inspur/driver.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/inspur/driver.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/inspur/sysinfo.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/inspur/sysinfo.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/intel/driver.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/intel/driver.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/intel/sysinfo.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/intel/sysinfo.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/utils.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/utils.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/xilinx/driver.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/xilinx/driver.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/fpga/xilinx/sysinfo.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/fpga/xilinx/sysinfo.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/gpu/base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/gpu/base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/gpu/nvidia/driver.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/gpu/nvidia/driver.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/gpu/nvidia/sysinfo.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/gpu/nvidia/sysinfo.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/gpu/utils.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/gpu/utils.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/modules/generic.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/modules/generic.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/nic/base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/nic/base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/nic/intel/driver.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/nic/intel/driver.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/nic/intel/sysinfo.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/nic/intel/sysinfo.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/qat/base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/qat/base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/qat/intel/driver.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/qat/intel/driver.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/qat/intel/sysinfo.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/qat/intel/sysinfo.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/nvmf/nvmf.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/nvmf/nvmf.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/spdk.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/spdk.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/util/common_fun.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/util/common_fun.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/util/pyspdk/nvmf_client.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/util/pyspdk/nvmf_client.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/util/pyspdk/py_spdk.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/util/pyspdk/py_spdk.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/util/pyspdk/vhost_client.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/util/pyspdk/vhost_client.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/spdk/vhost/vhost.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/spdk/vhost/vhost.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/ssd/base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/ssd/base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/ssd/inspur/driver.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/ssd/inspur/driver.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/ssd/inspur/sysinfo.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/ssd/inspur/sysinfo.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/accelerator/drivers/ssd/utils.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/accelerator/drivers/ssd/utils.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/agent/manager.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/agent/manager.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/agent/resource_tracker.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/agent/resource_tracker.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/agent/rpcapi.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/agent/rpcapi.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/__init__.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/__init__.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/app.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/app.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/config.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/config.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/controllers/base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/controllers/link.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/link.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/controllers/root.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/root.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/controllers/types.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/types.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/controllers/utils.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/utils.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/controllers/v2/__init__.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/controllers/v2/arqs.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/v2/arqs.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/controllers/v2/deployables.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/v2/deployables.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/controllers/v2/device_profiles.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/v2/device_profiles.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/controllers/v2/devices.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/v2/devices.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/controllers/v2/utils.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/v2/utils.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/controllers/v2/versions.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/controllers/v2/versions.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/expose.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/expose.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/hooks.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/hooks.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/middleware/__init__.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/middleware/auth_token.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/middleware/auth_token.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/middleware/parsable_error.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/middleware/parsable_error.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/rest_api_version_history.rst` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/rest_api_version_history.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/api/wsgi_app.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/api/wsgi_app.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/cmd/__init__.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/cmd/agent.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/cmd/agent.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/cmd/api.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/cmd/api.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/cmd/conductor.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/cmd/conductor.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/cmd/dbsync.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/cmd/dbsync.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/cmd/status.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/cmd/status.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/common/authorize_wsgi.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/common/authorize_wsgi.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/common/config.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/common/config.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/common/constants.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/common/constants.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/common/exception.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/common/exception.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/common/i18n.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/common/i18n.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/common/nova_client.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/common/nova_client.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/common/paths.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/common/paths.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/common/placement_client.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/common/placement_client.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/common/policy.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/common/policy.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/common/rpc.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/common/rpc.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/common/service.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/common/service.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/common/utils.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/common/utils.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/conductor/handlers.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/conductor/handlers.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/conductor/manager.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/conductor/manager.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/conductor/rpcapi.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/conductor/rpcapi.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/conf/__init__.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/conf/agent.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/conf/agent.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/conf/api.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/conf/api.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/conf/database.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/conf/database.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/conf/default.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/conf/default.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/conf/devices.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/conf/devices.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/conf/glance.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/conf/glance.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/conf/keystone.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/conf/keystone.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/conf/nova.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/conf/nova.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/conf/opts.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/conf/opts.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/conf/placement.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/conf/placement.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/conf/service_token.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/conf/service_token.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/conf/utils.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/conf/utils.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/context.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/context.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/db/__init__.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/db/__init__.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/db/api.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/db/api.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/db/migration.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/db/migration.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/env.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/env.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/4cc1d79978fc_add_ssd_type.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/4cc1d79978fc_add_ssd_type.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/7e6f1f107f2b_add_qat_type.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/7e6f1f107f2b_add_qat_type.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/899cead40bc9_add_nic_type.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/899cead40bc9_add_nic_type.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/c1b5abada09c_update_for_nova_integ.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/c1b5abada09c_update_for_nova_integ.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/d6f033d8fa5b_add_quota_related_tables.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/d6f033d8fa5b_add_quota_related_tables.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/ede4e3f1a232_new_db_schema.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/ede4e3f1a232_new_db_schema.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic/versions/f50980397351_initial_migration.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic/versions/f50980397351_initial_migration.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/alembic.ini` & `openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/alembic.ini`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/api.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/api.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/migration.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/migration.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/db/sqlalchemy/models.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/db/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/hacking/checks.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/image/api.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/image/api.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/image/glance.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/image/glance.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/__init__.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/arq.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/arq.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/attach_handle.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/attach_handle.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/attribute.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/attribute.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/control_path.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/control_path.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/deployable.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/deployable.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/device.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/device.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/device_profile.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/device_profile.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/driver_objects/driver_attach_handle.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/driver_objects/driver_attach_handle.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/driver_objects/driver_attribute.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/driver_objects/driver_attribute.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/driver_objects/driver_controlpath_id.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/driver_objects/driver_controlpath_id.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/driver_objects/driver_deployable.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/driver_objects/driver_deployable.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/driver_objects/driver_device.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/driver_objects/driver_device.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/ext_arq.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/ext_arq.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/extarq/ext_arq_job.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/extarq/ext_arq_job.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/extarq/fpga_ext_arq.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/extarq/fpga_ext_arq.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/objects/fields.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/objects/fields.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/policies/__init__.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/policies/base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/policies/base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/policies/device_profiles.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/policies/device_profiles.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/privsep/__init__.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/privsep/__init__.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/quota.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/quota.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/service_auth.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/service_auth.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/post_mortem_debug.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/post_mortem_debug.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/__init__.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/aichip/huawei/test_ascend.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/aichip/huawei/test_ascend.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/inspur/test_driver.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/inspur/test_driver.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/intel/prepare_test_data.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/intel/prepare_test_data.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/intel/test_driver.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/intel/test_driver.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/test_base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/test_base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/fpga/xilinx/test_driver.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/fpga/xilinx/test_driver.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/gpu/nvidia/test_driver.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/gpu/nvidia/test_driver.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/gpu/test_base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/gpu/test_base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/gpu/test_utils.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/gpu/test_utils.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/nic/intel/prepare_test_data.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/nic/intel/prepare_test_data.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/nic/intel/test_driver.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/nic/intel/test_driver.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/nic/test_base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/nic/test_base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/qat/intel/prepare_test_data.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/qat/intel/prepare_test_data.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/qat/intel/test_driver.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/qat/intel/test_driver.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/qat/test_base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/qat/test_base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/spdk/nvmf/test_nvmf.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/spdk/nvmf/test_nvmf.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/spdk/vhost/test_vhost.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/spdk/vhost/test_vhost.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/ssd/test_base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/ssd/test_base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/ssd/test_utils.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/ssd/test_utils.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/test_driver.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/test_driver.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/accelerator/drivers/test_fake_driver.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/accelerator/drivers/test_fake_driver.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/agent/test_resource_tracker.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/agent/test_resource_tracker.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/agent/test_rpcapi.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/agent/test_rpcapi.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/api/base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/test_api.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/test_api.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/test_arqs.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/test_arqs.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/test_deployables.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/test_deployables.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/test_device_profiles.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/test_device_profiles.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/test_devices.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/test_devices.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/test_fpga_program.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/test_fpga_program.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/api/controllers/v2/test_microversion.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/api/controllers/v2/test_microversion.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/cmd/test_status.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/cmd/test_status.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/common/test_nova_client.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/common/test_nova_client.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/conductor/test_manager.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/conductor/test_manager.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/db/base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_db_api.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_db_api.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_db_attach_handle.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_db_attach_handle.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_db_attribute.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_db_attribute.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_db_control_path.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_db_control_path.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_db_deployable.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_db_deployable.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_db_device.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_db_device.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_db_device_profile.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_db_device_profile.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_db_extarq.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_db_extarq.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/db/test_migrations.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/db/utils.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/db/utils.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/fake_attach_handle.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_attach_handle.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/fake_attribute.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_attribute.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/fake_deployable.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_deployable.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/fake_device.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_device.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/fake_device_profile.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_device_profile.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/fake_driver_device.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_driver_device.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/fake_extarq.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_extarq.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/fake_physical_function.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_physical_function.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/fake_virtual_function.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/fake_virtual_function.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/image/test_glance.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/image/test_glance.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_attach_handle.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_attach_handle.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_control_path.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_control_path.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_deployable.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_deployable.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_device.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_device.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_device_profile.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_device_profile.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_ext_arq_job.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_ext_arq_job.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_extarq.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_extarq.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_fpga_ext_arq.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_fpga_ext_arq.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/objects/test_objects.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/objects/test_objects.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/policies/base.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/policies/base.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/policies/test_device_profiles.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/policies/test_device_profiles.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/policy_fixture.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/policy_fixture.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/services/_test_placement_client.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/services/_test_placement_client.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/test_exception.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/test_exception.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/tests/unit/test_hacking.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/tests/unit/test_hacking.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg/version.py` & `openstack-cyborg-9.0.0.0rc1/cyborg/version.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/cyborg.conf.intelnic.sample` & `openstack-cyborg-9.0.0.0rc1/cyborg.conf.intelnic.sample`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/devstack/lib/cyborg` & `openstack-cyborg-9.0.0.0rc1/devstack/lib/cyborg`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/devstack/plugin.sh` & `openstack-cyborg-9.0.0.0rc1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/devstack/settings` & `openstack-cyborg-9.0.0.0rc1/devstack/settings`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/api_samples/accelerator_requests/accelerator_requests-after-update-resp.json` & `openstack-cyborg-9.0.0.0rc1/doc/api_samples/accelerator_requests/accelerator_requests-after-update-resp.json`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/api_samples/accelerator_requests/accelerator_requests-before-update-resp.json` & `openstack-cyborg-9.0.0.0rc1/doc/api_samples/accelerator_requests/accelerator_requests-before-update-resp.json`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/api_samples/accelerator_requests/accelerator_requests-create-resp.json` & `openstack-cyborg-9.0.0.0rc1/doc/api_samples/accelerator_requests/accelerator_requests-create-resp.json`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/api_samples/accelerator_requests/accelerator_requests-getone-resp.json` & `openstack-cyborg-9.0.0.0rc1/doc/api_samples/accelerator_requests/accelerator_requests-getone-resp.json`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/api_samples/accelerator_requests/accelerator_requests-list-resp.json` & `openstack-cyborg-9.0.0.0rc1/doc/api_samples/accelerator_requests/accelerator_requests-list-resp.json`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/api_samples/accelerator_requests/accelerator_requests-patch-curl.json` & `openstack-cyborg-9.0.0.0rc1/doc/api_samples/accelerator_requests/accelerator_requests-patch-curl.json`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/api_samples/deployables/deployables-getone-resp.json` & `openstack-cyborg-9.0.0.0rc1/doc/api_samples/deployables/deployables-getone-resp.json`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/api_samples/deployables/deployables-list-resp.json` & `openstack-cyborg-9.0.0.0rc1/doc/api_samples/deployables/deployables-list-resp.json`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/api_samples/device_profiles/device_profiles-create-resp.json` & `openstack-cyborg-9.0.0.0rc1/doc/api_samples/device_profiles/device_profiles-create-resp.json`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/api_samples/device_profiles/device_profiles-getone-resp.json` & `openstack-cyborg-9.0.0.0rc1/doc/api_samples/device_profiles/device_profiles-getone-resp.json`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/api_samples/device_profiles/device_profiles-list-resp.json` & `openstack-cyborg-9.0.0.0rc1/doc/api_samples/device_profiles/device_profiles-list-resp.json`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/api_samples/device_profiles/device_profiles-post-curl-with-bitstream.json` & `openstack-cyborg-9.0.0.0rc1/doc/api_samples/device_profiles/device_profiles-post-curl-with-bitstream.json`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/api_samples/device_profiles/v22/device_profiles-getone-resp.json` & `openstack-cyborg-9.0.0.0rc1/doc/api_samples/device_profiles/v22/device_profiles-getone-resp.json`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/api_samples/devices/devices-getone-resp.json` & `openstack-cyborg-9.0.0.0rc1/doc/api_samples/devices/devices-getone-resp.json`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/api_samples/devices/devices-list-resp.json` & `openstack-cyborg-9.0.0.0rc1/doc/api_samples/devices/devices-list-resp.json`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/admin/config-wsgi.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/admin/config-wsgi.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/admin/index.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/admin/index.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/cli/cyborg-status.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/cli/cyborg-status.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/conf.py` & `openstack-cyborg-9.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/configuration/policy-concepts.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/configuration/policy-concepts.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/configuration/policy-guide.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/configuration/policy-guide.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/configuration/policy.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/configuration/policy.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/configuration/sample-config.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/configuration/sample-config.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/configuration/sample-policy.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/configuration/sample-policy.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/contributor/contributing.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/contributor/devstack_setup.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/contributor/devstack_setup.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/contributor/driver-development-guide.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/contributor/driver-development-guide.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/contributor/index.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/contributor/microversions.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/contributor/microversions.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/contributor/releasenotes.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/contributor/releasenotes.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/contributor/rest_api_version_history.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/contributor/rest_api_version_history.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/figures/cyborg-architecture.png` & `openstack-cyborg-9.0.0.0rc1/doc/source/figures/cyborg-architecture.png`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/figures/cyborg-nova-interaction-workflow.svg` & `openstack-cyborg-9.0.0.0rc1/doc/source/figures/cyborg-nova-interaction-workflow.svg`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/figures/cyborg-nova-interaction.png` & `openstack-cyborg-9.0.0.0rc1/doc/source/figures/cyborg-nova-interaction.png`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/index.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/install/common.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/install/common.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/install/install-from-source.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/install/install-from-source.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/reference/driver-table.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/reference/driver-table.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/reference/support-matrix.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/reference/support-matrix.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/user/architecture.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/user/architecture.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/doc/source/user/introduction.rst` & `openstack-cyborg-9.0.0.0rc1/doc/source/user/introduction.rst`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/etc/cyborg/api-paste.ini` & `openstack-cyborg-9.0.0.0rc1/etc/cyborg/api-paste.ini`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/openstack_cyborg.egg-info/PKG-INFO` & `openstack-cyborg-9.0.0.0rc1/openstack_cyborg.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: openstack-cyborg
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Distributed Acceleration Management as a Service
 Home-page: https://docs.openstack.org/cyborg/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ======
         Cyborg
```

### Comparing `openstack-cyborg-9.0.0/openstack_cyborg.egg-info/SOURCES.txt` & `openstack-cyborg-9.0.0.0rc1/openstack_cyborg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/openstack_cyborg.egg-info/entry_points.txt` & `openstack-cyborg-9.0.0.0rc1/openstack_cyborg.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/openstack_cyborg.egg-info/requires.txt` & `openstack-cyborg-9.0.0.0rc1/openstack_cyborg.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/releasenotes/notes/cyborg-nova-interaction-8fe4e49e3c9b3b7b.yaml` & `openstack-cyborg-9.0.0.0rc1/releasenotes/notes/cyborg-nova-interaction-8fe4e49e3c9b3b7b.yaml`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/releasenotes/notes/implement_oslo_privsep-4fc6e15360c92772.yaml` & `openstack-cyborg-9.0.0.0rc1/releasenotes/notes/implement_oslo_privsep-4fc6e15360c92772.yaml`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/releasenotes/notes/policy-file-default-value-change-de14a3688357b081.yaml` & `openstack-cyborg-9.0.0.0rc1/releasenotes/notes/policy-file-default-value-change-de14a3688357b081.yaml`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/releasenotes/notes/policy_refresh_base_and_device_profile-cef00fca580d2323.yaml` & `openstack-cyborg-9.0.0.0rc1/releasenotes/notes/policy_refresh_base_and_device_profile-cef00fca580d2323.yaml`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/releasenotes/notes/remove-OPAE-dependency-from-devstack-f6db83bb37761340.yaml` & `openstack-cyborg-9.0.0.0rc1/releasenotes/notes/remove-OPAE-dependency-from-devstack-f6db83bb37761340.yaml`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/releasenotes/source/conf.py` & `openstack-cyborg-9.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/requirements.txt` & `openstack-cyborg-9.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/setup/roles/generate_credentials/tasks/main.yml` & `openstack-cyborg-9.0.0.0rc1/setup/roles/generate_credentials/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/setup/roles/install_package/tasks/main.yml` & `openstack-cyborg-9.0.0.0rc1/setup/roles/install_package/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/setup.cfg` & `openstack-cyborg-9.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/setup.py` & `openstack-cyborg-9.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/test-requirements.txt` & `openstack-cyborg-9.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/tools/check-cherry-picks.sh` & `openstack-cyborg-9.0.0.0rc1/tools/check-cherry-picks.sh`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/tools/flake8wrap.sh` & `openstack-cyborg-9.0.0.0rc1/tools/flake8wrap.sh`

 * *Files identical despite different names*

### Comparing `openstack-cyborg-9.0.0/tox.ini` & `openstack-cyborg-9.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

