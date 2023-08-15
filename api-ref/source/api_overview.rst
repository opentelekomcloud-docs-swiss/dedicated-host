:original_name: deh_03_0000.html

.. _deh_03_0000:

API Overview
============

You can use all DeH functions by making calls to the APIs provided by the DeH service, for example, allocating DeHs, querying the DeH list, viewing DeH details, and releasing a DeH.

.. table:: **Table 1** APIs

   +------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | API                          | Description                                                                                                                                                               |
   +==============================+===========================================================================================================================================================================+
   | Allocating DeHs              | Allocate one or more DeHs and set required parameters, such as the flavor, AZ, and quantity. The number of allocatable DeHs depends on the DeH quota owned by the tenant. |
   +------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | Querying DeHs                | Query the DeH list. You can add parameters such as **flavor**, **dedicated_host_id**, and **state** to the URI to filter the result.                                      |
   +------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | Querying Details About a DeH | Query details about a DeH, such as its name, AZ, number of available vCPUs, and available memory size.                                                                    |
   +------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | Querying ECSs on a DeH       | Query information about the ECSs deployed on a DeH, such as the names, IDs, and status of the ECSs.                                                                       |
   +------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | Modifying DeH Attributes     | Change the name of a DeH and enable or disable the auto placement function. After auto placement is enabled, ECSs can be automatically scheduled to this DeH.             |
   +------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | Releasing a DeH              | Released a DeH that is no longer used.                                                                                                                                    |
   +------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | Querying Available DeH Types | Query available DeH types in an AZ.                                                                                                                                       |
   +------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | Querying API Versions        | Query all available API versions and the versions of specified APIs.                                                                                                      |
   +------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | DeH Tag Management           | Add or delete tags for DeHs and query DeHs by tag.                                                                                                                        |
   +------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | Quota Configuration          | Query the DeH quota of a tenant.                                                                                                                                          |
   +------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. note::

   For details about the APIs for creating ECSs on DeHs, see the *Elastic Cloud Server API Reference*.
