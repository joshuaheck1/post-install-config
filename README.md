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
      <img width="1000" alt="PI2" src="https://github.com/user-attachments/assets/cf2543c2-9760-4806-920b-83b24e39a760" />
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







<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
