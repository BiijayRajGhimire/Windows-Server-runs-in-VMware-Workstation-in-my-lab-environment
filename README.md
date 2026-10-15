# Windows-Server-runs-in-VMware-Workstation-in-my-lab-environment host website 
use Public FREE SSL Certificate and ensure you can access website using https://serverIP
•	Add Web Server Role and Features in Server2
<img width="858" height="611" alt="image" src="https://github.com/user-attachments/assets/0aea61d1-3b5c-46d9-96f9-732b69dbe0c2" />

• Open notepad as admin
•	Host a website by creating isstart.htm file
•	Browse localhost or IP address in Server2
<img width="975" height="338" alt="image" src="https://github.com/user-attachments/assets/a80db231-ccda-4325-b972-a632ad5fe44c" />

•	Added A record in godaddy.com
<img width="975" height="316" alt="image" src="https://github.com/user-attachments/assets/5db41068-1d40-48d5-a61d-657e467fbc7f" />

•	In personal PC, run ping domain name. (ping www.ITsolutionconsulting.shop for Testing purpose
<img width="975" height="538" alt="image" src="https://github.com/user-attachments/assets/2d48d958-2f12-4535-8d21-9699b48a7abb" />

•	In Router change reserved http and https port 443 to 4433 and 80 to 8080.
<img width="975" height="280" alt="image" src="https://github.com/user-attachments/assets/8f881b25-9bd8-4d28-be97-f0ec81f2b8b0" />

•	Configure PAT rule/add Port Forward Rule 
<img width="975" height="387" alt="image" src="https://github.com/user-attachments/assets/8afd0830-5a88-4cdc-8344-f87e8e8657bb" />

•	From Personal PC – browse website ‘‘www.ITsolutionconsulting.shop” (unsecure website)
<img width="975" height="338" alt="image" src="https://github.com/user-attachments/assets/be24ddeb-7617-4769-ad19-320cd63f5e81" />

•	In Server2, go to Internal Information System (IIS) Manager,
Binding
Http port 80
Add IP address of server 2 and host name (192.168.1.10 www.ITsolutionconsulting.shop)
<img width="603" height="668" alt="image" src="https://github.com/user-attachments/assets/54b04de0-ce01-4993-b50a-125be643fc5c" />
<img width="850" height="530" alt="image" src="https://github.com/user-attachments/assets/26e28d38-27c6-4571-9a04-0da40896e31c" />

•	 Download Win-Acme from www.win-acme.com  to obtain public certificate for secure website. (Browse in server2 to download in server 2. Not in personal PC)
<img width="975" height="273" alt="image" src="https://github.com/user-attachments/assets/dc8a6734-e4d2-481f-b434-e656fbb90335" />

•	From downloaded file, 
Extract
Then run
<img width="836" height="826" alt="image" src="https://github.com/user-attachments/assets/7e9d9260-22db-435c-8d96-2ee18182734b" />
<img width="688" height="367" alt="image" src="https://github.com/user-attachments/assets/4165a71e-89af-46ba-8cc9-a6ae5be3e6ec" />
<img width="622" height="338" alt="image" src="https://github.com/user-attachments/assets/f7cfe7e6-b017-4a74-b298-05740e87bf8d" />
<img width="763" height="250" alt="image" src="https://github.com/user-attachments/assets/c5196027-edb7-48cf-b697-bddca89f6c58" />
<img width="975" height="537" alt="image" src="https://github.com/user-attachments/assets/469c156f-6c02-4b9f-99d4-7144c461d17e" />
<img width="975" height="572" alt="image" src="https://github.com/user-attachments/assets/957c6c14-69a7-469b-99b0-91974f0b2a39" />
•	In Server 2, in IIS, we can see port 443 has been auto added.
<img width="975" height="536" alt="image" src="https://github.com/user-attachments/assets/7fdd0a28-8579-4454-91e8-2bad6f4d3cc6" />

•	Add Port Configure Rule for Port 443 in Router
<img width="975" height="280" alt="image" src="https://github.com/user-attachments/assets/a29a52bb-ec4b-46e5-bfab-cebd58172f5c" />

Port forwarding TCP 80/443

<img width="975" height="360" alt="image" src="https://github.com/user-attachments/assets/418eba7a-2136-4e9f-8968-beab91c0319f" />

•	In Personal PC, browse Https://ITsolutionconsulting.shop(secure web browser)
<img width="975" height="519" alt="image" src="https://github.com/user-attachments/assets/ae4b05ea-7c4a-4f4f-86af-64973b32552f" />

