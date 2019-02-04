LDAP (Active Directory)
=======================

You can configure **Policy Server** to integrate with **Active Directory** for **User Authentication**

#. Go to **Preferences** in the top panel
#. Go to **User Authentication > Authentication Integration** in the left Preferences panel
#. Find **LDAP Authentication Integration** section in the main window
#. Enter the following:

   - **Server Address**:
   - **Server Port**: (*LDAP=389, LDAPS=636*)
   - **Base DN**: (*e.g. CN=Users,DC=company,DC=com*)
   - **Bind DN**: (*Should be FQDN: e.g. Administrator@company.com*) (*Bind Account should have Administrator Privileges*)
   - **Bind Password**:
   - **User Naming Attribute**: (*e.g. sAMAccountName*)
   - **SSL Connection**: (*Turn on if using LDAPS*)

#. Click **Update**
#. Click **Test** to test configuration settings (*Test account can be any User Account found within the Base DN*)

Troubleshooting
---------------

* Error Message **"LDAP Server connection failed. URI=ldaps://[IP]:[PORT]/, ERRMSG='-1:Can't contact LDAP server, TLSv1.0=-1:Can't contact LDAP server' "**

 * Possible Fix: Update LDAP Server Firmware to latest patches. Known issues authenticating against Active directory over Secure LDAP on unpatched servers due to encrytpion compatibility.  
