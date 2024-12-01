# Installing Docker and Peppermint in Linux Mint 22

<h2>Description</h2>
In this IT Help Desk task, I installed Docker on my Linux Mint 22 Desktop and successfully logged into the Peppermint ticketing dashboard. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>Linux CLI</b>
- <b>Perplexity AI</b> 

<h2>Environments Used </h2>

- <b>Linux Mint 22</b> 

<br />
<br />
I first tried to install it using the Ubuntu|Docker instructions but did not switch the version codename to Ubuntu codename. That may have fixed my initial issue.

![1 1) using perplexcity AI to find specific CLI for linux mint 22](https://github.com/user-attachments/assets/963deb37-b2eb-4068-88fb-abb89a2f3920)

<br />
<br />
Regardless, following perplexity AI's output for installing Docker on Linux Mint 22 helped me troubleshoot the issue.   

![1 2) using perplexcity AI to find specific CLI for linux mint 22](https://github.com/user-attachments/assets/a5fc3502-4244-4cf3-829d-4929a4380d70)

<br />
<br />
Ran hello world to confirm installation. 

![2) docker hello-world](https://github.com/user-attachments/assets/3b7efd78-03b2-4c71-9562-764f16060eae)

<br />
<br />
Created /peppermint directory in /home directory and wrote in the yml file. 

![3) mkdir peppermint   vi dockeryml](https://github.com/user-attachments/assets/8478d972-309e-44b5-bb00-dc38bca12645)

<br />
<br />
It's important to note that the Version 3.1 configuration file on docs.peppermint.sh/docker website did not include the API URL. 
I had trouble reaching the site since the URL wasn't configured. I manually inserted the API URL and replaced the hostname with "localhost".

![4) confirm docker yaml is written, don't forget api url](https://github.com/user-attachments/assets/ac8c4f45-7fe3-4f42-be08-e8763fabea33)

<br />
<br />
I ran "sudo docker compose up" not the suggested "docker-compose up -d" from the docs.peppermint.sh/docker website since those command did not work for me. 

![5) run docker compose](https://github.com/user-attachments/assets/70867219-0856-41dd-b1b5-f66afbac35aa)

<br />
<br />
Logged into the server with default logins from docs.peppermint.sh/docker website. 
The address was http://localhost:3000 not localhost:5003 in the YML file while Docker is running. 
Success.  

![6) login successful](https://github.com/user-attachments/assets/2d5a9d94-72b1-41e0-9035-e046055607b6)

<br />
<br />
