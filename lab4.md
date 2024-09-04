lab 4.1<br />![GWCQUAfXsAAZS5r](https://github.com/user-attachments/assets/52a22b0d-e3fd-42e8-a5b2-3cb3fa1e0ffc)
**Simulation of Alert triage and prioritization**

1)List of Alert to work on<br />
<br />
![GWCOoGxW0AAmsE-](https://github.com/user-attachments/assets/33f24ee4-4135-48a6-ab4e-8b0ba2b6e5fd)<br />
2)Working According to Cyber kill chainExfiltration is at top so we will first check that and verify
<br />
<br />
![GWCO0deWcAEm39e](https://github.com/user-attachments/assets/1844d8ed-59f6-473c-a308-d1dc5c5d6ca4)<br />
Can see there is Data transfer internally ..... looks like Social Security numbers<br />
<br />
![GWCPHEHWgAA78j_](https://github.com/user-attachments/assets/82d740c1-c3fd-4db2-b53e-716a597c9183)<br />
3) Checking Debugger Alert
But can see it is just Googles update Nothing more <br />
![GWCPdKPWAAAsrGK](https://github.com/user-attachments/assets/20c38070-852f-4097-a448-4ffd45d15bca)
<br />
<br />
4)Checking another EXE alert via HTTP<br />
<br />
![GWCP6AyWUAATjY1](https://github.com/user-attachments/assets/ae958586-7a68-432a-9b9a-6276c481efbb)<br />
Can see that it is zip file and if we check in virus total it gives malicious file<br />
![GWCP9hBWgAAZ-hG](https://github.com/user-attachments/assets/6067762f-f332-4010-a8be-10529c15a286)<br />

5)Checking remaning alert ... and can see all are same IP but one has different NetFlowID <br />
![GWCQUAfXsAAZS5r](https://github.com/user-attachments/assets/23591b7a-f870-4798-bb64-d0087034aeb6)<br />
![GWCQXzbXoAIokij](https://github.com/user-attachments/assets/394eba06-5f7a-420d-b4d6-b4ebbe3aeea4)<br />

Thus can merge all in one (it downlaods malicous exe) and has 2 EXE and 2 policy alert <br />
![GWCQqy0WIAAuF7d](https://github.com/user-attachments/assets/b6bf0ac3-bfa6-4ea2-8a8a-c9a7a6d57a5c)<br />
<br /><br /><br /><br /><br />
lab 4.2<br />

To: SOC@sec450.com<br/>
From: Jim@sec450.com<br/>
Subject: Possible infection<br/>
Hello - This morning (2019-04-11 roughly 8:45AM US Eastern) experienced a full-screen error message with a red background and audio alert, claiming a Microsoft infection. Did hard reboot and was fine.<br/>

![GVMD-oFXAAAHb4z](https://github.com/user-attachments/assets/152b7529-3d3e-493c-ac9c-ec96dacaa32f)<br />
seeing http event on SIEM system for more info (attack was at 8:37 - 8:46 <br />
![GVMEJ27WgAAaEbx](https://github.com/user-attachments/assets/edea90b2-a113-4a87-9124-1792a868e3e7)<br />
Searching more found that it had mp3 GET (via HTTP) as was said in letter.<br />
![GVMEjaPWEAAXkhM](https://github.com/user-attachments/assets/cb4336b8-7ee5-47ba-9c88-88e6a7006bee)<br />
Checking for new process (All of them were either System32/SystemApp) all need privilege escalation not possible within few minutes. Conclusion no harmful new process
![GVME4U-XUAEhMhs](https://github.com/user-attachments/assets/b57e0213-9e09-4394-bd05-0882ccd18ba0)
<br />
Checking for any virus from Windows defender .. but no ID 1116 on log thus no malware detected can be concluded<br />
![GVMFTUGWgAAdWN6](https://github.com/user-attachments/assets/eff25098-f052-4428-bf0b-b1328e9ff792)
<br />
Gave number on template ACH most likely Fake AV<br />
![GVMFpwWWAAAVAZI](https://github.com/user-attachments/assets/785fc8fd-06de-471b-8f5e-91e16cd7298b)
<br />

<br /><br /><br /><br /><br />

lab 4.3 <br />
Got the Alert on SIEM for some blocked Geo location trying to connect to Website<br />
![GVStf4lWMAAtF_g](https://github.com/user-attachments/assets/36dd442a-130f-4ad5-9a02-805a3300abfd)<br />
We searched and got that via this link mike was moved to some website aalayamdesigns[.]com from where the pass and user name was stolen<br />
![GVSt8G-XcAA58EZ](https://github.com/user-attachments/assets/b110dff3-4e6a-4d15-8579-ada2b360666e)<br />
Resolving alert on TheHive platform to complete the playbook<br />
![GVSuc87WUAAZhHO](https://github.com/user-attachments/assets/f8ca319e-de9c-4651-8f1e-a5cec1a7fed5)<br />
Giving more IOC that was not raised as alert after analysis for future<br/>
![GVSus-5XwAAUmWt](https://github.com/user-attachments/assets/4816c632-bdc5-4062-b688-123b84b9aeeb)





