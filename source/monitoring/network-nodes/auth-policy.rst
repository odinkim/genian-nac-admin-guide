Configuring Authentication Policy for Node Policy
=================================================

Node Authentication policies determine when and how nodes of a given group will be required to authenticate, as well as the conditions of the process.

To configure authentication policy options, select a node policy under **Policy > Node Policy > [Policy Name]** and scroll down to **Advanced > Authentication** in the main panel to access the following options:


Authentication Methods
----------------------

Select:

* **Host Authentication** - Authentication by device identifiers or network identifier such as MAC and IP Addresses. 

 or 

* **Password Authentication** 
 

Single Sign-On Method
---------------------

* Select: **Disable**, **Active Directory**, **External API**, or **Genian API** - (Agent Required)
 
 *  If **Active Directory**, Specify: Domain Name
 
Auth User Group
---------------

* Specify a user group that must be authenticated.

Auto-Logout
-----------

* Specify length of **Hour(s)**, **Day(s)**, **Week(s)**, or **Month(s)** a node can remain authenticated after a user login. 

Auto-Logout for Down Node
-------------------------

* Specify length of **Minute(s)**, **Hour(s)**, **Day(s)**, **Week(s)**, or **Month(s)** a node can remain authenticated not being detected.

Reauthentication Interval
---------------------------

* Specify **Everyday**, **Weekly**, or **Monthly** **Day** and **Time** to require reauthentication, or select **Not Specified** to not require Reauthentication.

Session Timeout Notification
----------------------------

* Specify **Minute(s)**, **Hour(s)**, **Day(s)**, **Week(s)**, or **Month(s)** previous to session expiration to notify user. - (Agent Required) 

Custom User Login Page URL
--------------------------

* Specify: **URL** that captive web portal login button will redirect to. 
 
Authentication at Startup
-------------------------

* Option to require authentication when the computer restarts or wakes. - (Agent Required)
 
 * Select: **On**, or **Off**

Display Name for Username
-------------------------

* Specify: Sample text in user sign in form. 

Display Name for Password
-------------------------

* Specify: Sample text in user sign in form. 

User Account Request
--------------------

* Option to display user account request option in captive web portal.
 
 * Select: **On**, or **Off**. 

 * If **On**, specify a Registration page, or leave blank for the default Registration page and select **On**, or **Off** for displaying a consent page.
