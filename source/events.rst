Managing Logs and Events
------------------------

Policy Server provides a centralized Log View.
Policy Server collects system and security related events to generate logs from endpoint devices, network devices, and other third-party devices.
From here, Logs can then be sent outwards to another storage location, such as a SIEM solution. 

Log view consists of four main sections.

- Panel A: Predefined Logs that are categorized by severity, frequently used, and RADIUS.
- Window B: Time Graph and Chart.
- Panel C: Status and Filter.
- Window D: Result window of your searching and filtering.

Log display and generation options may be configured under **General > Log** in the **Preferences** section. 

.. image:: /images/Log-View-Lettered.png
   
.. toctree::
   :maxdepth: 1

   logs/logs
   logs/sending-events
   logs/receiving-events
   logs/report