**lab 5.1**<br />
Initial message for filtering the logs<br />
![GVh8922XgAAMa3T](https://github.com/user-attachments/assets/04c400bd-24e0-4003-ab41-5eafa233910a)<br />

SIEM dashboard fired up<br />

![GVh9JOTXYAAn-gS](https://github.com/user-attachments/assets/7e124d96-0794-45de-8308-8f1023fb5d21)<br />

Web Server was running so filtered for port 80 443 <br />
![GVh9T9tW4AAJJ9v](https://github.com/user-attachments/assets/1965046c-956b-4cf5-a2a7-7fff52f1e204)<br />

Then filtering out source ip which was of the same machine so not that usefull according to instruction or finding we got<br/>
![GVh9ibyWkAA_nHz](https://github.com/user-attachments/assets/ff46d3b0-06f9-41e4-bba6-c4536b883bba)<br />

Filtering out generic alerts make more that half of alerts<br />

![GVh-Du8W8AA7Gqb](https://github.com/user-attachments/assets/9a3cd389-c749-4570-83b1-a4e82544b11b)<br />

Filtering out policy alert(ET Policy) as not mentioned that scan should be seen<br />
![GVh-NzzX0AEqWW4](https://github.com/user-attachments/assets/643491c4-e138-4b71-af41-0c0c441d0b4a)<br />


Final alert which is of value that should be investigated and improvised further<br />
![GVh-gvwWMAA7yNf](https://github.com/user-attachments/assets/fdd77a0b-c3a7-4b04-abce-599b5615a258)<br />
<br /><br /><br /><br />
**lab5.2**<br />

Simulation of SOAR using NODE-RED.
This node created for checking if new file was made<br />
![GVmNGbXWgAAsaz7](https://github.com/user-attachments/assets/6f080287-ed59-4557-8f9a-16d653a0b900)<br />
This node will check that if new was created or not and return true or false<br />
![GVmNW5yW4AAyQ5f](https://github.com/user-attachments/assets/7624632e-2d17-4c76-8c54-22448144f3a7)<br />
This node will be used to generate md5 hash of the new file<br />
![GVmNn-SXoAA2Q-G](https://github.com/user-attachments/assets/4808344c-190b-490e-b71e-db9a4224d274)<br />
Using this http request to send API and verify that if something was found or not using threat crowd API<br />
![GVmN2m8W4AAg-3f](https://github.com/user-attachments/assets/43e380db-8eee-437f-86b4-635f3883025b)<br />
Using the API result to verify if there is some threat or not<br />
![GVmOJBwWEAAYymt](https://github.com/user-attachments/assets/79c02a6d-fdee-46ad-a698-62d942bd705f)<br />
Giving message to email if found error<br />
![GVmOVeoXoAA0Chx](https://github.com/user-attachments/assets/9188b36e-81e1-45df-8b6b-90511d3152f9)<br />
Using the container environment to send message but no mail for first sample but for second there is.<br />
![GVmOmVlWsAAbikd](https://github.com/user-attachments/assets/37feb802-62f5-4df3-9671-9b1747b9ded5)<br />
![GVmO0QcWgAA0jW-](https://github.com/user-attachments/assets/9c8841d6-2fe8-4907-8e35-379ca53f924a)<br />
<br /><br /><br /><br />


**lab5.3**<br />

Work flow automation simulation using node-red and blocking ip in local server using simple form for easy work <br />
1)Dig at weather. com<br />

![GV_uVdLXEAA87yt](https://github.com/user-attachments/assets/a76845fc-a968-40a7-b2c5-5f863aedee90)<br />
Block form for any analyst to respond<br />
![GV_uhdEW8AAbWZB](https://github.com/user-attachments/assets/4ded33f0-8bb1-41c4-98f6-8f80ab20a243)<br />
this is the work flow of the automation process ( though done on node-red)<br />
![GV_urFRWoAApkXH](https://github.com/user-attachments/assets/2a737cec-d1e0-4d6e-b8c6-2f05ea0d0825)<br />
Blocking a weather. com IP as it is bad traffic (response phase )Note*<br />
![GV_u-JNWgAAkbpG](https://github.com/user-attachments/assets/4206e8ba-d7c8-4e35-a6aa-2b3a6ea350ad)<br />
It is blocked as we can see<br />
![GV_vMUwWYAAqz6Q](https://github.com/user-attachments/assets/77cd10d7-f3b7-416f-aeb3-15e1ca71fc2d)<br />


*It is done manually as no free software to implement


















