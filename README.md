- 👋 Hi, I’m @mraassis
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
mraassis/mraassis is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->


The Sh interface is defined by 3GPP in TS 29.329 as a diameter interface between an AS and HSS.

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
