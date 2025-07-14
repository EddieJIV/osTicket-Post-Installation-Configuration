# osTicket-Post-Installation-Configuration

*This lab will outline the post-install configuration of the open source help desk ticketing system osTicket prior to working mock-tickets in the next lab*

## Enviornments & Technologies Used:

* Microsoft Azure
* Windows 10 OS
* Remote Desktop
* IIS (Internet Information Services)
* osTicket

## Post Install Configuration Objectives:

1. [Agent](https://docs.osticket.com/en/latest/Agent%20Panel.html) vs. [Admin](https://docs.osticket.com/en/latest/Admin%20Panel.html) panel acknowledgement
2. [Role](https://docs.osticket.com/en/latest/Admin/Agents/Roles.html) Configuration 
3. [Department](https://docs.osticket.com/en/latest/Admin/Agents/Departments.html) Configuration
4. [Team](https://docs.osticket.com/en/latest/Admin/Agents/Teams.html) Configuration
5. [Agent](https://docs.osticket.com/en/latest/Admin/Agents/Agents.html) & [User](https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html) Configuration
6. [Service Level Agreement](https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html) Configuration
7. [Help Topic](https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html) Configuration

### Prerequisites: 

-  [osTicket Prereqisites](https://github.com/EddieJIV/osticket-prereqs)

## 1. Acknowledge Agent vs. Admin Panel 

Admin/Analyst Login Page:
http://localhost/osTicket/scp/login.php 

---

<img src="https://github.com/user-attachments/assets/dfc51e3b-9437-41c5-b169-0e12d2d49586" height="700" width="700" alt="Admin Panel"/>

#### Admin Panel on osTicket:
The **Admin Panel** in osTicket is the backend interface where administrators manage the overall configuration of the ticketing system. It allows admins to set up user roles, manage departments, configure email settings, customize ticket fields, and generate reports. Essentially, it is used for system administration and configuration.

<img src="https://github.com/user-attachments/assets/3dab8a1d-cfc3-4c00-9a33-90ab6111715a" height="700" width="700" alt="Agent Panel"/>

#### Agent Panel on osTicket:
The **Agent Panel** is the interface used by support agents to handle incoming support tickets. Agents can view, respond to, and manage tickets assigned to them or their department. This panel provides tools for communication with customers, tracking ticket status, and collaborating with other agents.

#### Key Differences:
- **Purpose**: The Admin Panel is for system configuration and management, while the Agent Panel is for handling and responding to support tickets.
- **User Role**: The Admin Panel is accessed by administrators, whereas the Agent Panel is accessed by support agents.
- **Functionality**: Admins can customize settings and manage users, while agents focus on ticket resolution and customer interaction.

These distinctions help ensure that the system is both well-managed and responsive to customer needs.

## 2. Role Configuration
*To define and manage the permissions and access levels for different agent roles within the system.*

<img src="https://github.com/user-attachments/assets/efea663e-9214-4b55-b51b-6df3783d5c2e" height="700" width="700" alt="Roles"/>

- First, we are going to navigate to the Role Confguration page under the Admin panel.
  - Admin Panel > Agents > Roles
- Click, "Add New Role"

<p>
  <img src="https://github.com/user-attachments/assets/b3800554-2323-43d2-91af-a30daac1bc5e" height="600" width="450" alt="Supreme Admin"/>
  <img src="https://github.com/user-attachments/assets/e8caa6c8-d508-405e-a8b7-3abbb195fe5e" height="600" width="450" alt="Permissions"/>
</p>

- Give the title of this new role "Supreme Admin"
- Move on to the Permissions tab, and check every box under the tickets, tasks, and knowledgebase sections. Effectively giving this new Supreme Admin role full access to do absolutely everything.
- click add role.

## 3. Department Configuartion
*To organize support agents into specific groups based on their roles, expertise, or the types of tickets they handle.*

<img src="https://github.com/user-attachments/assets/697d6675-9e7b-4209-9ce5-4060a3878942" height="700" width="700" alt="Departments"/>

<img src="https://i.imgur.com/DJmEXEB.png" height="700" width="700" alt="Placeholder Image"/>

<img src="https://i.imgur.com/DJmEXEB.png" height="700" width="700" alt="Placeholder Image"/>

<img src="https://i.imgur.com/DJmEXEB.png" height="700" width="700" alt="Placeholder Image"/>

<img src="https://i.imgur.com/DJmEXEB.png" height="700" width="700" alt="Placeholder Image"/>

<img src="https://i.imgur.com/DJmEXEB.png" height="700" width="700" alt="Placeholder Image"/>

<img src="https://i.imgur.com/DJmEXEB.png" height="700" width="700" alt="Placeholder Image"/>

<img src="https://i.imgur.com/DJmEXEB.png" height="700" width="700" alt="Placeholder Image"/>

<img src="https://i.imgur.com/DJmEXEB.png" height="700" width="700" alt="Placeholder Image"/>

<img src="https://i.imgur.com/DJmEXEB.png" height="700" width="700" alt="Placeholder Image"/>

<img src="https://i.imgur.com/DJmEXEB.png" height="700" width="700" alt="Placeholder Image"/>

<img src="https://i.imgur.com/DJmEXEB.png" height="700" width="700" alt="Placeholder Image"/>

<img src="https://i.imgur.com/DJmEXEB.png" height="700" width="700" alt="Placeholder Image"/>

<img src="https://i.imgur.com/DJmEXEB.png" height="700" width="700" alt="Placeholder Image"/>

<img src="https://i.imgur.com/DJmEXEB.png" height="700" width="700" alt="Placeholder Image"/>

<img src="https://i.imgur.com/DJmEXEB.png" height="700" width="700" alt="Placeholder Image"/>

<img src="https://i.imgur.com/DJmEXEB.png" height="700" width="700" alt="Placeholder Image"/>

<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="600" width="450" alt="Placeholder Image"/>
  <img src="https://i.imgur.com/DJmEXEB.png" height="600" width="450" alt="Placeholder Image"/>
</p>


<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="600" width="450" alt="Placeholder Image"/>
  <img src="https://i.imgur.com/DJmEXEB.png" height="600" width="450" alt="Placeholder Image"/>
</p>


<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="600" width="450" alt="Placeholder Image"/>
  <img src="https://i.imgur.com/DJmEXEB.png" height="600" width="450" alt="Placeholder Image"/>
</p>

<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="600" width="450" alt="Placeholder Image"/>
  <img src="https://i.imgur.com/DJmEXEB.png" height="600" width="450" alt="Placeholder Image"/>
</p>






