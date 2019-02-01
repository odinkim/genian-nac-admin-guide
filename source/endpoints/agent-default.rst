Configuring Agent Defaults
==========================

Agent default policies determine the basic installation and operation of the agent on endpoints.
Additional node specific agent settings may be additionally configured.See: :doc:`agent-node-policy`

To configure agent default options, select **Preferences** on the menu bar and **Agent** in the left panel.

Prompting for Installation
--------------------------

* Determines if the installer gives consent prompt to install agent when the installer is executed. (Windows Only)

 * Select: **On**,or **Off**

Installation Progress Bar
-------------------------

* Displays progress of installation. (Windows Only)
 
 * Select: **On**, or **Off**
 * If **On**, select **On**, or **Off** for installation result message.
 
Destination Folder
------------------

* Defines the location the agent files will be installed to. Default: %ProgramFiles%\Geni\Genian (Windows Only)

Network For Automatic Update
----------------------------

* Select Network Object to be used for agent updates.

Displaying in Control Panel
---------------------------

* Select: **On**, or **Off** for displaying agent under the Programs section in Control Panel. (Windows Only)

View My Status on Tray Menu
---------------------------

* Select: **On**, or **Off** for Tray/ Menu Bar Agent Icon info. (Windows and OSX only)

KeepAlive Interval
------------------

* Specify: **Second(s)**, or **Minute(s)** for communication interval to update Agent runtime log. 5 Missed communications will define the agent as not running. 

Scheduling Agent Restart
------------------------

* * Specify: **Minutes** **Hours** past computer entering sleep mode for the agent to reboot. (Windows and OSX only)
 
Hiding Address Bar / Toolbar
----------------------------

* Select: **Disable**, or **Enable** for Internet Explorer application control. (Windows only)

 * Select window size: **Normal**, or **Maximized**

SSL Certificate
---------------

* Select: **On**, or **Off** for installing SSL Certificate from the policy server. (Windows and OSX only)

Custom Icon
-----------

* Upload a custom image for the tray icon. (Windows only)


Network Service
---------------

* Specify a network object to enable the agent running.  (Windows only)




