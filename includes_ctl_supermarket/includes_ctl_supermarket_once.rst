.. The contents of this file are included in multiple topics.
.. This file describes a command or a sub-command for supermarket-ctl.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.


The supervisor for |supermarket| is configured to restart any service that fails, unless that service has been asked to change its state. The ``once`` subcommand is used to tell the supervisor to not attempt to restart any service that fails.

This command is useful when troubleshooting configuration errors that prevent a service from starting. Run the ``once`` subcommand followed by the ``status`` subcommand to look for services in a down state and/or to identify which services are in trouble. This command can also be run for an individual service by specifying the name of the service in the command.

This subcommand has the following syntax:

.. code-block:: bash

   $ supermarket-ctl once name_of_service

where ``name_of_service`` represents the name of any service that is listed after running the ``service-list`` subcommand.



