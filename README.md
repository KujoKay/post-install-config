<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket. It will also help with learning and understanding the basic configurations of osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles (for grouping permissions)
- Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
- Configure Teams
- Configure Agents (workers)
- Configure Users (customers)
- Configure SLA
- Configure Help Topics (For when users create a ticket)

<h2>Configuration Steps</h2>

<p>
1. If you haven't already, sign in to your osTicket Azure VM. From there, go to http://localhost/osTicket/scp/login.php and it will take you to the admin page. Use your admin credintals to sign in. Once you have signed in, you should be in the admin panel. From there, we will begin to configure roles. 
</p>
<p>
<img src="https://github.com/user-attachments/assets/68e9f5ea-c8a1-465e-b15e-1e237e9ef6be"/>
</p>
<br />

<p>
2. When you're in the admin panel, click on "Agents" then select "Roles". Once you do that, click "Add New Role" and name the new role "Supreme Admin". After naming the role, click on "Permissions" and make sure all the boxes are check off in "Tickets", "Tasks", and "Knowledgebase". Once that's done, click "Add Role" and the "Supreme Admin" role will be created!
</p>
<p>
<img src="https://github.com/user-attachments/assets/7c352c45-5ed4-4f0d-ba10-ee0db9fc68be"/>
<img src="https://github.com/user-attachments/assets/ac2c9bbd-7c23-4660-87cb-4f8526a04c89"/>
<img src="https://github.com/user-attachments/assets/e1cde134-0b02-46df-935f-f66f381afea0"/>
<img src="https://github.com/user-attachments/assets/324d9ef7-c427-458f-9f20-63ff5653e7c5"/>
</p>
<br />

<p>
3. Now that we have an understanding of roles, next is to configure departments. Click on "Departments" then "Add New Department". Once you do that, name the new department "SysAdmins". For the sake of this demonstration, you can ignore the other settings and click "Create Dept". Now you should have new department created!
</p>
<p>
<img src="https://github.com/user-attachments/assets/089a1e0f-aeea-45b7-89ae-250becd73396"/>
<img src="https://github.com/user-attachments/assets/15396a72-f558-42f4-90e3-4f87f8c3365f"/>
</p>
<br />

<p>
4. Next is to configure teams. Click on "Teams" then "Add New Team". Next, name the team "Online Banking" and click "Create Team." Now you should have a new team created!
</p>
<p>
<img src="https://github.com/user-attachments/assets/41dd331d-8130-44a5-a950-c70a55cfee9b"/>
<img src="https://github.com/user-attachments/assets/eb8e4147-5b38-4e27-be1b-6213d0757619"/>
</p>

<p>
5. Next, we will configure settings so anyone can create a ticket. Click on "Settings" then go to "Users". Under "Authentication Settings", make sure the "Require registration and login to create tickets" box is unchecked. 
</p>
<p>
<img src="https://github.com/user-attachments/assets/7fc97ef6-46d6-4650-9cec-43ed4d7109d1"/>
</p>

<p>
6. Now we will configure agents, or the workers. Click on "Agents" then navigate to the "Agents tab". Type in a first and last name and assign it an email address. Give the account a username and a password (in order to give the account a password, uncheck the "Send the agent a password reset email" and the prompts will appear). Once you do that, go to the "Access" tab and under "Primary Department", assign the "SysAdmins" department and "Supreme Admin" role to the account. In the "Permissions" tab, ensure all the boxes are checked. In the "Teams" tab, assign the account to "Online Banking" and click "Create". 
</p>
<p>
<img src="https://github.com/user-attachments/assets/5d25d050-24d3-4b93-8e71-65b27cfcc57d"/>
<img src="https://github.com/user-attachments/assets/0b7f0742-4c7f-49be-972d-027f0b694762"/>
<img src="https://github.com/user-attachments/assets/1fe150dc-f134-4978-9d9b-ae4a30f064c0"/>
<img src="https://github.com/user-attachments/assets/f045b868-bd24-4106-9edd-d2afa3babd2d"/>
<img src="https://github.com/user-attachments/assets/296da4f1-dee9-4f94-9c24-56777715b1ab"/>
</p>

<p>
7. Now we will configure the user accounts, or customers. Instead of being the admin panel, we must switch to the agent panel. On the top right, click "Agent Panel". Next, click "Users" then "Add user". Fill in the email address and name, then click "Add User". The account should like the secound image below. 
</p>
<p>
<img src="https://github.com/user-attachments/assets/1d8c2931-4b2a-49b7-b9b9-3cb8e7a57dcb"/>
<img src="https://github.com/user-attachments/assets/9a6cabaa-7a95-4009-8b97-de8d2190bda6"/>
</p>

<p>
8. Next, we will configure SLAs, or service-level agreements. Switch from "Agent Panel" back to "Admin Panel." Once you do that, click "Manage" then the "SLA" tab. Click on "Add new SLA Plan" to begin the process. Name the new plan "Sev-A", give 1 hour in the "Grace Period" column, and choose "24/7" in the "Schedule" column. Once all of that is done, click "Create". Now you have a new SLA plan! 
</p>
<p>
<img src="https://github.com/user-attachments/assets/f96dbe95-8326-4bcb-9841-b03d1eb17c8a"/>
<img src="https://github.com/user-attachments/assets/b9f04223-371b-47b7-ba3f-3e68394ad14b"/>
</p>

<p>
9. Lastly, we will configure Help Topics. This is to help users creating a ticket. Click on the "Help Topics" tab and click "Add New Help Topic". For the new topic, title it "Business Critical Outage" and select "Report a Problem" in the "Parent Topic" column. Once that is done, click "Add Topic" and a new help topic will be created.
</p>
<p>
<img src="https://github.com/user-attachments/assets/9e966357-cae2-41fc-a009-47c3b0a364b6"/>
<img src="https://github.com/user-attachments/assets/e0de07d4-4835-49e5-a5a9-190f56013ae5"/>
</p>
