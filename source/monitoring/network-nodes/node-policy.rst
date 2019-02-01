Configuring Management Policy for Node Policy
=============================================

To configure management policy options, select a node policy under **Policy > Node Policy > [Policy Name]** and scroll down to **Advanced > Management** in the main panel to access the following options:

Hostname Policy for New Node
----------------------------

* Determines if the policy server assigns a host name policy to new nodes. Host name policy is a mandate for the host name of a given node. Nodes whos host names are non compliant will be flagged in the management pane, and non compliance with host name policy can be used as a status group condition. 

 * Select: **On**,or **Off** 
 * If **On**, select Hostname Template. 

Deleting Node Down
------------------

* Specify: **Hour(s)**, **Day(s)**, **Week(s)**, or **Month(s)** from node downtime start to delete the node from the policy server. Enter **0** to disable.
 
CWP Design Template
-------------------

* Select which Captive Web Portal Design Template to display to nodes in this policy group.  