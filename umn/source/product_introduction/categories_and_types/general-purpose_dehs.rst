:original_name: deh_01_0006.html

.. _deh_01_0006:

General-Purpose DeHs
====================

Overview
--------

General-purpose DeHs can accommodate ECSs with regular workloads and short-term workload surges. They use a CPU-unbound scheduling scheme. vCPUs are randomly allocated to idle CPU hyper threads based on the system loads. If traffic loads are light, the computing performance is high. However, if traffic loads are heavy, vCPUs of different ECSs compete for physical CPU resources, resulting in unstable computing performance.

Currently, only the s3 DeH type equipped with the latest-generation Intel® Xeon® Skylake CPUs, providing better cost-effectiveness, is provided and can be used to deploy S3 ECSs.

DeH Specifications
------------------

.. table:: **Table 1** Specifications of s3 DeHs

   +-------------+--------------------------+--------------------------+---------------------------------------------------------------------------------------------+-----------------+
   | Flavor Type | Number of CPUs (Sockets) | Number of Physical Cores | Hardware Specifications                                                                     | Number of vCPUs |
   +=============+==========================+==========================+=============================================================================================+=================+
   | s3          | 2                        | 22                       | -  CPU: Intel® Xeon® Skylake 6161 v5 (frequency: 2.20 GHz; Turbo Boost frequency: 3.00 GHz) | 264             |
   |             |                          |                          | -  Memory: 702 GB (or 718,848 MB)                                                           |                 |
   +-------------+--------------------------+--------------------------+---------------------------------------------------------------------------------------------+-----------------+

ECSs Allowed on DeHs
--------------------

.. table:: **Table 2** ECS flavors allowed on s3 DeHs

   ============ ===== ===========
   ECS Flavor   vCPUs Memory (GB)
   ============ ===== ===========
   s3.medium.1  1     1
   s3.medium.2  1     2
   s3.medium.4  1     4
   s3.medium.8  1     8
   s3.large.1   2     2
   s3.large.2   2     4
   s3.large.4   2     8
   s3.large.8   2     16
   s3.xlarge.1  4     4
   s3.xlarge.2  4     8
   s3.xlarge.4  4     16
   s3.xlarge.8  4     32
   s3.2xlarge.1 8     8
   s3.2xlarge.2 8     16
   s3.2xlarge.4 8     32
   s3.2xlarge.8 8     64
   s3.4xlarge.1 16    16
   s3.4xlarge.2 16    32
   s3.4xlarge.4 16    64
   s3.4xlarge.8 16    128
   s3.8xlarge.1 32    32
   s3.8xlarge.2 32    64
   s3.8xlarge.4 32    128
   s3.8xlarge.8 32    256
   ============ ===== ===========
