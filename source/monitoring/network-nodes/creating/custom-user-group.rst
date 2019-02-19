Creating a Node Group from a Custom User Field
==============================================

In this article, we will show how to import a custom user field and use it to define a a node group. For this example we will use Active Directory group membership.

Configure a Custom User Field
-----------------------------

#. Go to **Preferences > Properties > Field Editor > User** and then **Task > Create.**
#. For **Key,** select ``CUSTOM01`` and define the **name**  as ``ADgroup`` or desired label and click **Save**.

Configure Data Synchronization
------------------------------
 
#. Go to **Preferences > User Authentication > Data Synchronization**
#. Fill out the Data Synchronization form using standard procedure as shown in :doc:`/authentication/synch-directory/ldap`  
#. Under **User Information > Collumn Name for 01** enter: ``$memberOF,substring_index(substring_index(substring_index($, ',', 1), ',', -1), '=', -1)``
#. Click **Update** at the bottom of the page, and then select the check box next to Syncronization ID, click the **Tasks** button in the upper left of the view window, and Click the **Synchronize Now** option. 

Create New User Group
---------------------

#. This new user group will be defined in relation the ``ADgroup`` value. 
#. Select the **Policy** tab at the top of the screen and click **Group > User** in the left menu panel. Select **Task > Create** to create a new user group.
#. Under **Condition** , select ``ADgroup``, define the **operater** and **value.** Click **Update,** and select **Apply** in the top right corner of the view pane.

Create New Node Group
---------------------

#. This node group will be defined as any node where the authenticated user, is one of the user group we have created. 
#. Select the **Policy** tab at the top of the screen and click **Group > Node** in thethe left menu panel. Select **Task > Create** to create a new policy group. 
#. Under **Condition** , select **Add**, define **Options** as **Auth User**, **Operater** as **is one of,** and **value** as the user group previously created.  Click **Add,** then click **Save.** Select **Apply** in the top right corner of the view pane.

