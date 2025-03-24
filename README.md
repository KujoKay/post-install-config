<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


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
<img src="https://github.com/user-attachments/assets/68e9f5ea-c8a1-465e-b15e-1e237e9ef6be"/>
</p>
<p>
1. If you haven't already, sign in to your osTicket Azure VM. From there, go to http://localhost/osTicket/scp/login.php and it will take you to the admin page. Use your admin credintals to sign in. Once you have signed in, you should be in the admin panel. From there, we will begin to configure roles. 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/7c352c45-5ed4-4f0d-ba10-ee0db9fc68be"/>
<img src="https://github.com/user-attachments/assets/ac2c9bbd-7c23-4660-87cb-4f8526a04c89"/>
<img src="https://github.com/user-attachments/assets/e1cde134-0b02-46df-935f-f66f381afea0"/>
<img src="https://github.com/user-attachments/assets/324d9ef7-c427-458f-9f20-63ff5653e7c5"/>
</p>
<p>
2. When you're in the admin panel, click on "Agents" then select "Roles". Once you do that, click "Add New Role" and name the new role "Supreme Admin". After naming the role, click on "Permissions" and make sure all the boxes are check off in "Tickets", "Tasks", and "Knowledgebase". Once that's done, click "Add Role" and the "Supreme Admin" role will be created!
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/089a1e0f-aeea-45b7-89ae-250becd73396"/>
<img src="https://github.com/user-attachments/assets/15396a72-f558-42f4-90e3-4f87f8c3365f"/>
</p>
<p>
3. Now that we have an understanding of roles, next is to configure departments. Click on "Departments" then "Add New Department". Once you do that, name the new department "SysAdmins". For the sake of this demonstration, you can ignore the other settings and click "Create Dept". Now you should have new department created!
</p>
<br />
