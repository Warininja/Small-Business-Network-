# How I built a Small Business network
Date: Feb 17, 2023
Dwaine Hood
-----
## Stage 1 Network Setup
I was asked to Build out a network infrastructure for a small business where the customer requested a LAN, Guest and DMZ network.
1. I first added the the devices to lab workspace in GN3
2. I then configured the LAN network on the firewall through the CLI over the console interface.
3. I added a Win10 workstation to the LAN network.
4. Connected to the firewall GUI from the Win10 workstation.
5. Completed the network setup through the firewall GUI.
![Stage 1 Network Setup](https://user-images.githubusercontent.com/123712481/219796115-50ba9f74-844e-4a29-b677-62025e81ad0e.png)
## Stage 2 Network Setup
In stage 2 I built a windows domain for the customers small business envirmonment.
1.  Prepared a Win2012r2 server for the “Active Directory Domain Services” server role.
2.  Installed the “Active Directory Domain Services” server role.
3.  Created new AD user accounts.
4.  Prepared Win10 to join the local domain.
5.  Joined Win10 to the local domain.
![Stage 2 Network Setup](https://user-images.githubusercontent.com/123712481/219798135-9189a00e-b521-4c22-9215-5ef36b662a36.png)
## Stage 3 Network Setup
Built a IIS webserver on Win2012r2 server, and joined the server to the domain
1.  Prepared Win2012r2 server to join the domain.
2.  Installed the “Internet Information Services” server role.
3.  Added a test webpage, and verified access over the LAN network.
![Stage 3 Network Setup](https://user-images.githubusercontent.com/123712481/219799491-a7a812fe-0fd6-4568-b83f-fff75a37e82d.png)
## Stage 4 Network Setup
Built a LAMP Webserver on Ubuntu server on the DMZ netwrok
1.  Prepared Ubuntu server.
2.  Installed DokuWiki.
3.  Configured DokuWiki.
4.  Setup a VIP for the public side of the webserver on the firewall.
![Stage 4 Network Setup](https://user-images.githubusercontent.com/123712481/219800624-bc4fd469-1e9d-4d5b-ba32-fff9d539d696.png)
## Stage 5 Network Setup
Built a FTP Server on a win2012r2 server on the DMZ netwrok.

1.   Prepared the win2012r2 server.
2.   Installed the FTP service.
![Stage 5 Network Setup](https://user-images.githubusercontent.com/123712481/219801157-056c44de-9d39-4f30-a1ab-1e48655d7d28.png)
## Stage 6 Hardened the enviroment
Researched how to harden the environment
1.  Added a page for notes in the wiki.
2.  Researched hardening a FortiGate firewall.
3.  Research hardening Windows 10.
4.  Research hardening Windows Server 2012r2.
5.  Research hardening Ubuntu server 18.04.
6.  Presented findings to my senior engineer.

[Research hardening a FortiGate firewall.docx](https://github.com/Warininja/testrepo/files/10772067/Research.hardening.a.FortiGate.firewall.docx)
## Stage 7 Scanning the environment
Conducted a vulnerability scan on the WAN interface and network environment
1.  Connected network to Greenbone server.
2.  Created a target of the WAN interface IP for the firewall.
3.  Scaned the target.
4.  Documented the results and submitted to my senior engineer.

[Vulnerabilty report.docx](https://github.com/Warininja/testrepo/files/10772098/Vulnerabilty.report.docx)
