Configuring Agent Defaults
==========================

Agent default policies are configured on the basis of individual node policies, which are then applied to node groups.
To configure agent defaults, select a node policy under **Policy > Node Policy > [Policy Name]** and scroll down to
**Advanced > Agent Policy** in the main panel to access the following options:

Agent
-----

* Specify: 

 * **On**, **Off**, or **Delete** to toggle agent run status or remove the agent from the node(s).


* Automatic Installation:

 * Select **On**, or **Off**, to toggle agent auto-installation from captive web portal window.


* Deleting Agent Not Running:

 * Define a time frame of **Hours**, **Days**, **Weeks** or **Months** upon which to Delete the agent, if it has not connected to the policy server. Input **0** to disable this function.


Agent Fail-safe
---------------

* Deactivates  the agent after a defined a time frame of **Minutes** **Hours**, **Days**, **Weeks** or **Months** since the agent has not been connected to the policy server.
 
 * Select **On**, or **Off**
 
Tray Icon
---------

* Toggles the appearance of the Agent Icon in the OSX Menu- Status Bar or the Windows System Tray.

 * Select **On**, or **Off**

Execution Account
-----------------

* Select **Computer Logon Account**, **Privileged Account**,or **Local System Account** to run the agent. Ensure the account selected has the proper permissions to perform agent actions configured under enforcement policy. See: :doc:`controlling-windows`, :doc:`controlling-macos`. 

 * **Computer Logon Account** - Runs the agent from whatever account is logged in. 

 * **Privileged Account** - Select this option for multiple devices within a domain to be used by non administators, and configure with domain administator credentials.

 * **Local System Account** - Select this account option for root level credentials on the local machine. Best used for node policies applied to a single device.

Policy Update Interval
----------------------

* Specify a time frame of **Hours** for the agent to check the policy server for updates.

 * Select between 1-4 **Hours**


Deleting Outdated Information
-----------------------------

* Define a time frame of **Hours**, **Days**, **Weeks** or **Months** upon which to Delete the agent information, if it has not connected been updated. Input **0** to disable this function.



