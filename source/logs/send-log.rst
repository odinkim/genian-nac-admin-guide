Sending Logs
============

You can send Events to external locations like SIEM solutions using several methods.

.. note:: Outbound email and admin email notification settings must both be configured.See :doc:`/system/email` , :doc:`/system/admin-account`

#. Select a **log filter**, click **edit**
#. Click **Checkbox** for **Notification** (Administrator email ), **Syslog**, **SNMP Trap**, or **Webhook**.
#. Configure settings and Update.

Example Integration: Splunk
---------------------------

Integrate with splunk using the following process:

1. In Splunk configure a Local UDP input under **Settings > Data Inputs**
2. Configure your desired **data input port** and enter your Genians policy server IP into the "Only accept connection from" section. (optional)
3. In Genians NAC, select syslog under the log filter of your choice.
4. For **Protocol**, select **UDP**, and for **server port**, select the **data input port** you defined on Splunk.
5. In the SYSLOG message section, enter the value {_DATETIME},LOGTYPE={_LOGTYPE},LOGID={_LOGID},IP={_IP},MAC={_MAC},MSG={_FULLMSG}, DETAIL={_DETAILMSG} 
 
 * This is necessary for the proper display of information in Splunk.
