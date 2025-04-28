<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Prerequisites</h2>

- [Creating Virtual Machines in the Cloud](https://github.com/joshuaheck1/VM-creation)

- [osTicket: Prerequisites and Installation](https://github.com/joshuaheck1/osticket-prereqs)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket

<h2>Operating Systems Used </h2>

- macOS Sequoia
- Windows 10 (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Section 1: Intro to URLs and Admin Panel vs Agent Panel
- Section 2: [Roles](https://docs.osticket.com/en/latest/Admin/Agents/Roles.html)
- Section 3: [Departments](https://docs.osticket.com/en/latest/Admin/Agents/Departments.html)
- Section 4: [Teams](https://docs.osticket.com/en/latest/Admin/Agents/Teams.html)
- Section 5: [Agents ](https://docs.osticket.com/en/latest/Admin/Agents/Agents.html)& [Users](https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html)
- Section 6: [Service Level Agreements (SLA)](https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html)
- Section 7: [Help Topics](https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html)

<h2>Configuration Steps</h2>

<h3>Section 1: Intro to URLs and Admin Panel vs Agent Panel</h3>

<table>
  <tr>
    <td>
      <img width="1000" alt="PI1" src="https://github.com/user-attachments/assets/faa074b0-ce78-4160-a5fa-884b85f5839d" />
    </td>
    <td>
      <img width="950" alt="PI2" src="https://github.com/user-attachments/assets/cf2543c2-9760-4806-920b-83b24e39a760" />
    </td>
  </tr>
</table>
<p>- osTicket has two main URLs that we will use during this project and the next one.</p>
<p>- http://localhost/osTicket/scp - Your Staff Control Panel. This is used by Admins and the Help Desk Agents. See Figure 1</p>
<p>- http://localhost/osTicket.com - Your osTicket URL. This is for end users to create tickets and check ticket status. See Figure 2</p>

<table>
  <tr>
    <td>
      <img width="1000" alt="PI3" src="https://github.com/user-attachments/assets/f9eb004d-3567-470c-b1d6-87d4dec82cee" />
    </td>
    <td>
      <img width="1000" alt="PI4" src="https://github.com/user-attachments/assets/0a2b3cf4-4ae9-43a4-9aa6-710325588676" />
    </td>
  </tr>
</table>
<p>- Once you're logged in to the Staff Control Panel URL, there are two different panels that can be used depending on your permissions.</p>
<p>- Admin Panel - This is used by the System Admin to confiured settings on the backend. </p>
<p>- Agent Panel - This is used by the Help Desk Agents or Support Specialists to view and work tickets.</p>
<p>- As an Admin, you can switch panels by clicking the panel name in the top right of the screen. We will be jumping between the two a lot during this project. Now, top off your coffee or grab another energy drink and lets get started. </p>

<h3>Section 2: Roles</h3>

<table>
  <tr>
    <td>
      <img width="996" alt="PI5" src="https://github.com/user-attachments/assets/e5cc5c49-2a22-4ace-b708-d34fe0df6a5d" />
    </td>
    <td>
      <img width="1000" alt="PI6" src="https://github.com/user-attachments/assets/d8ba554f-ddfc-4985-a821-3738fe940dc1" />
    </td>
  </tr>
</table>
<p>- Configure a new role within the Admin Panel. (Remember, "Agent Panel" will display in the top-right of your screen while in the Admin Panel.)</p> 
<p>- Within Admin Panel, click Agents -> Roles -> + Add New Role.</p> 
<p>- Name the new role "Supreme Admin" and click the Permissions tab.</p>
<br/>


<table>
  <tr>
    <td>
      <img width="1000" alt="PI7" src="https://github.com/user-attachments/assets/f5632967-ea12-44dd-8b93-26e3f682105f" />
    </td>
    <td>
      <img width="1000" alt="PI8" src="https://github.com/user-attachments/assets/02641de8-60f1-427e-b676-d0a21da0d1d0" />
    </td>
  </tr>
</table>
<p>- We want the Supreme Admin Role to have all the permissions for the sake of this project.</p>
<p>- Under Tickets, check all the boxes and click Tasks.</p>
<p>- Under Tasks, check all the boxes again and click Knowledgebase.</p>

<table>
  <tr>
    <td>
      <img width="1000" alt="PI9" src="https://github.com/user-attachments/assets/e87e2ef8-c613-4a98-925c-81b0edb954e3" />
    </td>
    <td>
      <img width="1000" alt="PI10" src="https://github.com/user-attachments/assets/1a731001-c945-4a61-b859-1d7377126507" />
    </td>
  </tr>
</table>
<p>- Under Knowledgebase, check all of the one box and click Add Role.</p>
<p>- The Supreme Admin Role was successfully added.</p> 
<p>- You can learn more about Roles within osTicket by clicking the link in the Post-Install Configuration Objectives above.<p/>
<p>- Next, we'll add a new Department.</p>

<table>
  <tr>
    <td>
      <img width="1000" alt="PI11" src="https://github.com/user-attachments/assets/772d618b-3fad-48bf-940a-e3f982b49607" />
    </td>
    <td>
      <img width="1000" alt="PI12" src="https://github.com/user-attachments/assets/65a769eb-fa93-4e87-b451-313259b93378" />
    </td>
  </tr>
</table>
<p>- Within Admin Panel, click Agents -> Departments -> + Add New Department.</p>
<p>- Under Settings, leave Parent as "Top-Level Department" and name the department "SysAdmins".</p>
<p>- This is all we'll do here for now. Ignore the Access tab for now because we still need to create some Agents. Scroll down and click Create.</p>
















<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
