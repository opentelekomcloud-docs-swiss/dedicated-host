:original_name: deh_02_0023.html

.. _deh_02_0023:

Modifying DeH Attributes
========================

Function
--------

This API is used to modify the **auto_placement** and **name** attributes of a DeH.

URI
---

PUT /v1.0/{project_id}/dedicated-hosts/{dedicated_host_id}

:ref:`Table 1 <deh_02_0023__table572214121015>` describes the parameters.

.. _deh_02_0023__table572214121015:

.. table:: **Table 1** Parameters description

   +-------------------+-----------------+-----------------+-----------------------------------------------------------------------------------------------------+
   | Parameter         | Type            | Mandatory       | Description                                                                                         |
   +===================+=================+=================+=====================================================================================================+
   | project_id        | String          | Yes             | Specifies the project ID.                                                                           |
   +-------------------+-----------------+-----------------+-----------------------------------------------------------------------------------------------------+
   | dedicated_host_id | String          | Yes             | Specifies the DeH ID.                                                                               |
   |                   |                 |                 |                                                                                                     |
   |                   |                 |                 | You can obtain the DeH ID from the DeH console or using the :ref:`Querying DeHs <deh_02_0020>` API. |
   +-------------------+-----------------+-----------------+-----------------------------------------------------------------------------------------------------+

Request
-------

-  Request parameters

   .. table:: **Table 2** Request parameters

      +----------------+-------------+-------------+-------------+-------------------------------------------------------------------------------------------------------------------------+
      | Parameter      | In          | Type        | Mandatory   | Description                                                                                                             |
      +================+=============+=============+=============+=========================================================================================================================+
      | auto_placement | in          | String      | No          | Specifies whether to allow an ECS to be placed on any available DeH if its DeH ID is not specified during its creation. |
      |                |             |             |             |                                                                                                                         |
      |                |             |             |             | The value can be **on** or **off**.                                                                                     |
      +----------------+-------------+-------------+-------------+-------------------------------------------------------------------------------------------------------------------------+
      | name           | in          | String      | No          | Specifies the DeH name.                                                                                                 |
      +----------------+-------------+-------------+-------------+-------------------------------------------------------------------------------------------------------------------------+

-  Example request

   .. code-block:: text

      PUT https://{Endpoint}/v1.0/9c53a566cb3443ab910cf0daebca90c4/dedicated-hosts/74259164-e63a-4ad9-9c77-a1bd2c9aa187
      {
          "dedicated_host": {
              "auto_placement": "off",
              "name": "DeH_vm3"
          }
      }

Response
--------

-  Response parameters

   None

-  Example response

   .. code-block::

      Http Response Code: 204

Status Code
-----------

See :ref:`Status Codes <deh_02_0016>`.
