
The Sh interface is defined by 3GPP in TS 29.329 as diameter interface between one or multiple Application Servers (AS) and the Home Subscriber Server (HSS).

The AS can use this interface to:
1) Query or update users data stored on HSS
2) Subscribe to receive notifications from the HSS of changes in users data

We will handle on this HLD only the scenario number 2, scenario number 1 can be supported but is out-of-scope.

The Sh interface specification, 3GPP TS 29.328, defines the IMS profile data that can be queried and updated via Sh. All user data accessible via the Sh interface is presented as an XML document with the schema defined in 3GPP TS 29.328.

For the scenario presented we

IMSUserState

IMS User State of the public identifier referenced. 
Its possible values are:
- REGISTERED,
- NOT_REGISTERED,
- AUTHENTICATION_PENDING,
- REGISTERED_UNREG_SERVICES. 




Subscription/notification procedures
– An AS can subscribe to receive notifications from the HSS of changes in data.
– The HSS can notify an AS of changes in data for which the AS previously had subscribed.

Application Layer Messages over Sh Interface

Subscribe-Notifications-Request (SNR) Command
The Subscribe-Notifications-Request (SNR) command, indicated by the Command-Code field set to 308 and the ‘R’ bit
set in the Command Flags field, is sent by the application server (AS) to the home subscriber server (HSS) in order to request notifications of
changes in user data. 

Subscribe-Notifications-Answer (SNA) Command
The Subscribe-Notifications-Answer command, indicated by the Command-Code field set to 308 and the ‘R’ bit cleared
in the Command Flags field, is sent by home subscriber server (HSS) in response to the Subscribe-Notifications-Request command. 

Push-Notification-Request (PNR) Command
The PNR command, indicated by the Command-Code field set to 309 and the ‘R’ bit set in the Command Flags field, is sent by HSS to the AS in order to notify changes in the subscribed user data. 

Push-Notifications-Answer (PNA) Command
The PNA command, indicated by the Command-Code field set to 309 and the ‘R’ bit
cleared in the Command Flags field, is sent by the AS in response to the PNR command from HSS.


References
https://www.etsi.org/deliver/etsi_ts/129300_129399/129329/07.06.00_60/ts_129329v070600p.pdf
https://www.etsi.org/deliver/etsi_ts/129300_129399/129328/06.13.00_60/ts_129328v061300p.pdf
https://www.3gpp.org/ftp/Specs/archive/29_series/29.329/
https://www.3gpp.org/ftp/Specs/archive/29_series/29.328/
