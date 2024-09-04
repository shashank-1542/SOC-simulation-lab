![GTYEnvUXIAMQrxr](https://github.com/user-attachments/assets/fed856b2-d55a-4b95-9469-d2799fc50f39)lab 3.1<br />
Windows Event log analysis in S.I.E.M(KIBANA)
![GWE8L0jWQAAZ_qd](https://github.com/user-attachments/assets/46c64f0f-10e7-454c-ae36-fb7d1f5a6f7e)<br />
Analysis on log using ip traffic <br />
1)All unsuccessful log are from one <IP> <br />
![GWE87u9WYAA9Y3T](https://github.com/user-attachments/assets/e78a8548-f375-4160-b474-f2bfced9b8d9)<br />
2)Port scan by the same machine(Both on the subnet maybe Exfiltration)<br />
![GWE9W0oXsAACsI1](https://github.com/user-attachments/assets/042dec05-ed27-4c86-a523-766dd8750064)
3)USB on the machine event id *6416*(USB device insertions .... in this case software{Bluetooth} see top secret)<br />
![GWE9xtlWIAAbo0n](https://github.com/user-attachments/assets/23fd05dd-45c2-466f-93da-b37f5ee955b9)<br />
4)Windows Anti Virus Alert Windows Defender Alert  Event ID 4663<br />
![GWE_IyTWgAE6GLg](https://github.com/user-attachments/assets/93a8fc5c-38d5-4324-a985-dd33a6c7997c)<br />
![GWE-0L2WoAE8TYT](https://github.com/user-attachments/assets/3a163008-5edd-4646-937d-4e7924c18632)<br />

<br /><br /><br /><br /><br />

lab 3.2 <br />
Different kind of log files (structred,unstructred and semi-structured)<br />
![GWFKkOqXcAAoymN](https://github.com/user-attachments/assets/4c7d7fb7-a76b-4429-967f-81ebd53b72fa)<br />
![GWFK2UmW4AIMOrW](https://github.com/user-attachments/assets/b7163c5a-6843-4216-8736-01e825e4328e)<br />

In this lab we simulate LOGAGENT and LOGSTASH behavior simulation <br />
In this video we see how log agent have the log there<br />
https://x.com/i/status/1828825521083585023<br />
In this nc is used as agent to transfer file over network<br />
![GWFT7ltWcAA-w8N](https://github.com/user-attachments/assets/a1aef3ef-cd0e-425b-9713-747740b19e4f)<br />
In this the LOGSTASH is normalized<br />
![GWFUHKoWQAA3s1o](https://github.com/user-attachments/assets/0b692978-2fa6-477c-a4a9-aed969ca8331)<br />
Geo Location is added<br />
![GWFUT8eWwAAYEyA](https://github.com/user-attachments/assets/5603b0a0-f4c8-4e20-a498-cfc3a469d996)<br />
Tag are added for making our search easy and quick<br />
![GWFUZ8jWsAA5i7O](https://github.com/user-attachments/assets/349551a2-95f0-4096-80a1-da8fe1ae5045)<br />

<br /><br /><br /><br /><br />

lab 3.3 <br />
Viewing an File Which may be Infected and than analysing different file and cases<br />
Unzip an infected file<br />
![GTYBgToXgAECHct](https://github.com/user-attachments/assets/18e6a858-125d-4cc6-a824-8301685e06df)<br/>
**Javascript file( obfuscated)** <br />
![GTYB_BzXUAAbeSm](https://github.com/user-attachments/assets/68cb679c-08e6-4803-8df9-13da6ae5a44b)<br />
**Checking .bin and .rtf file (these were ms office file before 2007)** <br />
windows exe on linux using olevba(Checking of any VBA) <br />
![GTYCQTXWkAAwS2_](https://github.com/user-attachments/assets/1b541f98-5351-4e15-9010-cf746727d07d)<br />
this one (decoding base 64 to view what the VBA does)>br />
![GTYCkVOXIAAPy3l](https://github.com/user-attachments/assets/e431a3f1-54f6-45ad-9f10-4bab83783db4)<br />
another windows but no VBA ..... then checking for **embedded**<br />
![GTYDJJtW4AADCLi](https://github.com/user-attachments/assets/ccc3db6b-053f-4d68-9d69-047a3729474d)<br />
Uing oleobj to analyse the .rtf file and there is some source included<br />
![GTYDeOuXkAAOZSZ](https://github.com/user-attachments/assets/96d7e53c-9f14-4b84-877e-d56ed2e770ab)<br />

**Analysing pdf file uising peepd.py**
![GTYEPiKWoAA8exE](https://github.com/user-attachments/assets/db37f919-b566-486b-994c-13d5ce570583)<br />
Obj[9] has uri (maybe malicious)
![GTYEcz8W0AAq-9k](https://github.com/user-attachments/assets/497a5595-3e9e-43eb-91e4-07fabe59124d)
Obj[40,58] has a javascript(maybe to execute some command)
![GTYEnvUXIAMQrxr](https://github.com/user-attachments/assets/27dfaca5-5d4b-46d3-accb-335216e47bf2)<br />
![GTYE05pWEAALu0O](https://github.com/user-attachments/assets/e0e79452-e7da-464e-9e27-418ab72a554a)<br /><br />
Hex dump of the file using -Cv for getting the ASCII  and gaps to get to know about what kind it is (MZ zip)<br />
![GTYE7LSX0AA8ohx](https://github.com/user-attachments/assets/ab669c5b-3fc3-4787-a098-f807aad2801c)<br />
Virus Total of the file (hash)<br />
![GTYFXQJXwAAGioV](https://github.com/user-attachments/assets/917d2744-601f-4ae2-9dc2-52a333dc3e6b) <br />
















