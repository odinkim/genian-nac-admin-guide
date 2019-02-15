Synchronizing User Directories
==============================

Additional information such as department, job title, email, and group is required if policy is to be established using the usage information.
If the user is not created locally but exists externally, this information should be retrieved via synchronization.
Additional information can be used to create user groups or use them as node group conditions.

.. toctree::
   :maxdepth: 1

   synch-directory/rdbms
   synch-directory/ldap
   synch-directory/csv

Testing Synchronization
-----------------------

#. Go to **Preferences** in the top panel
#. Go to **User Authentication > Data Synchronization** in the left Preferences panel
#. Select checkbox of desired configuration.
#. Click **Tasks > Synchronize Now**

You can check result through Logs