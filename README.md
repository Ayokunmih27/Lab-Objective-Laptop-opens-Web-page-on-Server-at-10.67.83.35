# Lab-Objective-Laptop-opens-Web-page-on-Server-at-10.67.83.35
Lab Objective:  Laptop opens Web page on Server at 10.67.83.35  
• Use VLAN 10 for the Laptop and Server.  
• VLAN 10 is supporting the IPv4 network of 10.67.83.32 /27  
  o Trunking is already configured between switches.  
  o DHCP services are already enabled for VLAN 10.
  
<img width="968" height="440" alt="Image" src="https://github.com/user-attachments/assets/7ca931d0-ccd2-406b-b3a7-2927622ff82f" />

 




**My Initial Observations**


•	On SW3, VLAN 10 was already configured, and the Server was connected to VLAN 10.

<img width="938" height="365" alt="Image" src="https://github.com/user-attachments/assets/c7d6a36b-1958-47f9-ad03-49073a788241" />

 


•	On SW1 and SW2, only the default VLAN was present.

<img width="943" height="296" alt="Image" src="https://github.com/user-attachments/assets/5aa25bc4-179f-4662-b8d1-0f9305f12d0a" />
<img width="938" height="325" alt="Image" src="https://github.com/user-attachments/assets/19196b02-825a-490a-a6eb-7762471592b7" />


•My Laptop was not in VLAN 10.

•	As a result, when I tried to open the Server’s web page, it failed.

<img width="924" height="592" alt="Image" src="https://github.com/user-attachments/assets/3a680df2-5dfa-4dc4-bf43-8d032017056c" />



**Steps I Took**

1. Configured VLAN 10 on SW1 and SW2:
Command

<img width="975" height="550" alt="Image" src="https://github.com/user-attachments/assets/378ca096-48ca-49a2-9bc6-7c1a7025b725" />
<img width="997" height="575" alt="Image" src="https://github.com/user-attachments/assets/d8c3609b-a49a-46c3-a77d-34c1caa14e48" />

2. Moved the Laptop’s interface into VLAN 10:

<img width="465" height="183" alt="Image" src="https://github.com/user-attachments/assets/3327ee7b-bb44-406b-93c1-3c856d2734f6" />
<img width="987" height="318" alt="Image" src="https://github.com/user-attachments/assets/875653d7-90e3-4279-b7cc-21e9d2b66c28" />

**Finally, I opened a browser on the Laptop → and successfully reached the Server’s web page.**

<img width="851" height="630" alt="Image" src="https://github.com/user-attachments/assets/fceebbf2-ef77-4d83-97d0-a665a3ec2dd1" />



