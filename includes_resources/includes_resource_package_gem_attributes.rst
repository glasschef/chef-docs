.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

This resource has the following attributes:

.. list-table::
   :widths: 150 450
   :header-rows: 1

   * - Attribute
     - Description
   * - ``clear_sources``
     - |clear_sources| Default value: ``false``.
   * - ``gem_binary``
     - |gem_binary resource package| By default, the same version of |ruby| that is used by the |chef client| will be installed.
   * - ``options``
     - |command options|
   * - ``package_name``
     - |name package| Default value: the ``name`` of the resource block. |see syntax|
   * - ``provider``
     - Optional. |provider resource_parameter| |see providers|
   * - ``source``
     - Optional. The URL at which the gem package is located.
   * - ``timeout``
     - |timeout|
   * - ``version``
     - |version package|
