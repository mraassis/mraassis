- 👋 Hi, I’m @mraassis
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
mraassis/mraassis is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->




Application Layer Messages over Sh Interface

Subscribe-Notifications-Request (SNR) Command
The Subscribe-Notifications-Request (SNR) command, indicated by the Command-Code field set to 308 and the ‘R’ bit
set in the Command Flags field, is sent by the application server (AS) to the home subscriber server (HSS) in order to request notifications of
changes in user data. 

Subscribe-Notifications-Answer (SNA) Command
The Subscribe-Notifications-Answer command, indicated by the Command-Code field set to 308 and the ‘R’ bit cleared
in the Command Flags field, is sent by home subscriber server (HSS) in response to the Subscribe-Notifications-Request command. 


Push-Notification-Request (PNR) Command
The Push-Notification-Request (PNR) command, indicated by the Command-Code field set to 309 and the ‘R’ bit set in
the Command Flags field, is sent by a Diameter server to a Diameter client in order to notify changes in the user data in
the server. 
