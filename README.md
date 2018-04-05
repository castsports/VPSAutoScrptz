# VPSAutoScrptz
Service:
OpenSSH: 22,444  
Dropbear: 143,3128  
SSL: 443  
Squid: 8000,8080
OpenVPNOpenVPN(TCP): 1194

Requirements:
Dedicated VPS Server (eg. DO,Vultr,Aruba,Linode,GoogleCloud)
VPS OS: Debian 7.11 32/64Bit (Never been Rebuild & No Previous Installation of VPS Service eg. SSH,VPN,OCS Panel etc.)
SSH Client: eg. Windows(Putty), Android(JuiceSSH)
SFTP Client: eg. Windows(Filezilla,WinSCP), Android(MiXplorer)
Your VPS IP must be Registered Here http://bytessh.ml/ocs/
Common Sense (Most Important)

Installation:
First: Gumawa muna ng Web Panel na paglalagyan ng mga server.
Need:
1 Debian 7.11 32|64 Bit (VPS)Droplet.
Steps:
Open Any SSH Client at Login mo Info ng (VPS)Droplet mo.
Paste this command Then Press Enter Key.
Code:
wget https://raw.githubusercontent.com/Clrkz/VPSAutoScrptz/master/OCSAutoScrptz.sh && chmod +x OCSAutoScrptz.sh && ./OCSAutoScrptz.sh
kung gusto mo gawing server din yung panel mo, Skip mo yung command sa taas at ito ang ilagay sa SSH Client:
Code:
wget https://raw.githubusercontent.com/Clrkz/VPSAutoScrptz/master/VPSnOCScrptZ.sh && chmod +x VPSnOCScrptZ.sh && ./VPSnOCScrptZ.sh
Type mo yung gusto mo maging Password at Name ng MySQL Database mo.
Hintayin hanggang may mag message sa SSH Client. at Follow nyo lang yung mga next step dun.

Second: Gumawa ng Servers na ilalagay sa Web Panel.
Need:
Another Debian 7.11 Droplet.
Steps:
Open Any SSH Client at Login mo Info ng (VPS)Droplet mo.
Paste this command Then Press Enter Key.
Code:
wget https://raw.githubusercontent.com/Clrkz/VPSAutoScrptz/master/VPScrptZ.sh && chmod +x VPScrptZ.sh && ./VPScrptZ.sh
Hintayin Hanggang Matapos.

Third: ilagay ang nagawang Server sa Web Panel.
Steps:
mag login sa ginawang WebPanel gamit ang credentials na nilagay mo.
In Menu Click Servers and select Add server.
Sundin lang kung ano yung nakalagay sa Panel.
Pwede ka maglagay ng kahit ilang server sundin lang ulit yung Second Instruction

Fourth: Gumawa ng users na gagamit ng Panel at server mo.
Steps:
Click Menu -> Users -> Add User
Sundin lang kung ano yung nakalagay sa Panel
kung Gusto mong idisable ang pag change password ng user, open your SSH Client then paste this Command:
Code:
wget https://raw.githubusercontent.com/Clrkz/VPSAutoScrptz/master/DsblChngPW.sh && chmod +x DsblChngPW.sh && ./DsblChngPW.sh

Fifth: Change Web Panel Contents (eg. Design, Image, Files: kelangan may alam kayo kahit konti sa HTML at PHP)
Steps:
Open Any SFTP Client and Login your VPS(Droplet) Info.
Navigate to /home/vps/public_html
Makikita mo na lahat ng files/contents ng Webpanel mo at pwede mo na itong Baguhin using some text editor eg.: notepad,notepad++
Kayo na bahala mag explorein

Sixth: Edit/Update Server message
Steps: 
Open Any SSH Client and Login your Droplet(VPS) Info.
Paste this command Then Press Enter Key.
Code:
nano /etc/issue.net
pwede mo nang palitan yung mga contents ng server message depende sa gusto mo.

Seventh: How to change user accounts Registration Days Limit
Open Any SFTP Client and Login your VPS(Droplet) Info.
Pumunta sa /home/vps/public_html/view/admin/ at hanapin ang file na account.html ilagay ito sa local storage eg.internal external storage o sa any local drives, iopen ito using any text editor (Windows:Notepad,Notepad++)(Android:DroidEdit,QuickEdit) Hanapin ang "+30 Days" at palitan ang number 30 depende sa gusto mo.
Pumunta sa /home/vps/public_html/controller/member/ hanapin ang file na server.php, iopen using any text editor at palitan ang "+30 Days" depende sa gusto mo.

