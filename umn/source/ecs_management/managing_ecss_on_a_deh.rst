:original_name: deh_01_0024.html

.. _deh_01_0024:

Managing ECSs on a DeH
======================

Scenarios
---------

You can start, stop, restart, or delete ECSs on a DeH on the management console.

Procedure
---------

#. Log in to the management console.

#. Click |image1| in the upper left corner and select the desired region and project.

#. Under **Computing**, click **Dedicated Host**.

   The **Dedicated Host** page is displayed.

#. Click the name of the target DeH.

   The DeH details page is displayed.

#. On the **ECSs on the DeH** tab, locate the target ECS and select the target option in the **Operation** column to manage the ECS. Alternatively, select the target ECSs and select an operation above the ECS list.

   The options are as follows:

   -  **Modify Specifications** (allowed only when ECSs are stopped)
   -  **Start** (allowed only when ECSs are stopped)
   -  **Stop** (allowed only when ECSs are running)
   -  **Restart** (allowed only when ECSs are running)
   -  **Delete**
   -  **Migrate ECS** (allowed only when ECSs are stopped)

Related Operations
------------------

On the **ECSs on the DeH** tab page, you can also click to create ECSs.

For details, see Elastic Cloud Server User Guide.

.. note::

   -  When selecting an ECS type, pay attention to mapping between the ECS type and the DeH type. If no matched DeH resources exist, ECSs cannot be created.

.. |image1| image:: /_static/images/en-us_image_0210485079.png
