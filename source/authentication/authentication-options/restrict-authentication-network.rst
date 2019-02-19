Restricting Authentication to a Specific Network
================================================

The network sensor IP can be used as a condition to assign the nodes to a node group. This group can be assigned to a Node Policy with authentication restrictions based on User Group. With this setup, nodes on a given network, will only allow users from the specified group to authenticate.  

Create New Node Group
---------------------

#. Go to the **Policy** tab at the top of the screen and click **Group > Node** in the left menu panel. Select **Tasks > Create Policy Group** to create a new policy group. 
#. Under **Condition** , select **Add**, define **Options** as ``Sensor``, **Operater** as ``is equal to,`` and **value** as the ``Sensor IP`` of the network to be controlled.  
#. Click **Add,** then click **Save.** Select **Apply** in the top right corner of the view pane.

Create New Node Policy
----------------------
 
#. Go to **Policy.** Select **Tasks > Create** in the top left of the view pane. 
#. Fill out the Node policy wizard up to the **Node Group** tab using standard procedure as shown in :doc:`/monitoring/network-nodes/node-policy`.
#. Under **Node Group** select the node group created by the Network Sensor IP.
#. Under **Policy Preferences > Auth User Group,** select the ``User Group`` that will be allowed to authenticate on nodes impacted by this policy.
#. Click **Apply** in the top right corner of the management pane.

