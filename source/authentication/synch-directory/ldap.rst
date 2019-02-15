LDAP (Active Directory)
=======================

.. note:: This feature requires Enterprise Edition

Genian NAC can use an LDAP directory as a source of user and organization information. LDAP synchronization allows user accounts to be created locally
and used for administration or policy. LDAP synchronization is commonly used with Microsoft Active Directory (AD) systems.

The following describes how to synchronize user and organizational information based on AD.

Creating Synchronization
------------------------

#. Go to **Preferences** in the top panel
#. Go to **User Authentication > Data Synchronization** in the left Preferences panel
#. Click **Tasks > Create**

Under **General**

#. For **ID**, type unique name.
#. For **Update Interval**, select the specified time or periodic interval for this Synchronization.
#. For **Applying Policy**, select ``Enabled`` for applying change after Synchronization. If there are several synchronization settings, you can set it to Disabled and enable only the last one.

Under **Database**

#. For **Type**, section ``LDAP``
#. For **Server Address**, type IP Address or FQDN of Active Directory server
#. For **Server Port**, type AD LDAP service port. by default LDAP port is ``389``. if you use LDAPS (LDAP over SSL) default port is ``636``.
#. For **SSL Connection**, select ``On`` if you use LDAPS.
#. For **DB Username**, type Bind DN of Active Directory. normally, you can use email format like administrator@company.com
#. For **DB Password**, type Bind DN user's password

Under **User Information**

#. For **Table Name**, type base distinguished name (DN) of users. normally, CN=Users,DC=company,DC=com
#. For **Where Clause for DB**, type ``(&(objectClass=user)(objectCategory=person))`` for filtering person object.
#. For **Column Name for Username**, type ``sAMAccountName``
#. For **Column Name for Full Name**, type ``displayName``
#. For **Column Name for Department**, type ``$distinguishedName, IF(LOCATE('OU=',$)>0,SUBSTRING($,LOCATE(',',$)+1),'')``
#. For any other extra information, you can use LDAP attribute name for each column name.

Under **Department Information**

#. For **Table Name**, type base distinguished name (DN) of organizationUnit (OU). normally, DC=company,DC=com
#. For **Where Clause for DB**, type ``objectClass=organizationalUnit`` for filtering OU object.
#. For **Sort Criteria**, type ``@NAMEPATH`` for ordering based on department name.
#. For **Column Name for Department ID**, type ``distinguishedName``
#. For **Column Name for Department**, type ``name``
#. For **Column Name for Parent Dept.**, type ``$distinguishedName, SUBSTRING($,LOCATE(',',$)+1)``
#. Click **Save** at the bottom

Testing Synchronization
-----------------------

#. Go to **Preferences** in the top panel
#. Go to **User Authentication > Data Synchronization** in the left Preferences panel
#. Select checkbox of desired configuration.
#. Click **Tasks > Synchronize Now**

You can check result through Logs

.. attention:: Since the Active directory does not provide the userPassword attribute, the user password can not be synchronized. Therefore, you must set the integration separately. See :doc:`../integrate-external/active-directory` 
