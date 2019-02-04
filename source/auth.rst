Managing User Authentication
----------------------------

.. note:: This feature requires Professional or Enterprise Edition

User Authentication means verifying the identity of someone (User) behind a device that wants to access the network. User Authentication also enables accountability, by using user ID and password which makes it possible to link access and actions to specific identities. Genians provides the ability to Authenticate Users in several ways.

You can create Users locally in Policy Server, or configure Policy Server to pull User Information from Active Directory, RADIUS, POP3, IMAP, SMTP, CSV, or other third-party user management systems.

**Locally**
Users Authenticate against the local database created within the Genians Policy Server. Once credentials match, the user is then allowed to proceed onto the network.

**Externally** (*Active Directory, RADIUS, IMAP, POP3, SMTP, CSV*)
Genians can integrate with External Authentication sources to permit user access upon successful login using proper credentials.

* Version 5.0.16: Cloud hosted Policy Server Authentication and Synchronization against private IP database currently not supported. 

.. toctree::
   :maxdepth: 1

   authentication/enabling-authentication
   authentication/managing-users
   authentication/integrate-external
   authentication/synch-directory
   authentication/authentication-options   
   