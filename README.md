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
2. [Roles](https://docs.osticket.com/en/latest/Admin/Agents/Roles.html)
3. [Departments](https://docs.osticket.com/en/latest/Admin/Agents/Departments.html)
4. [Teams](https://docs.osticket.com/en/latest/Admin/Agents/Teams.html)
5. [Agents](https://docs.osticket.com/en/latest/Admin/Agents/Agents.html) & [Users](https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html)
6. [Service Level Agreements](https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html)
7. [Help Topics](https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html)

### Prerequisites: 

-  [osTicket Prereqisites](https://github.com/EddieJIV/osticket-prereqs)

## 1. Acknowledge Agent vs. Admin Panel 

Admin/Analyst Login Page:
http://localhost/osTicket/scp/login.php 

---

<img src="https://github.com/user-attachments/assets/dfc51e3b-9437-41c5-b169-0e12d2d49586" height="700" width="700" alt="Admin Panel"/>

### Admin Panel on osTicket
The **Admin Panel** in osTicket is the backend interface where administrators manage the overall configuration of the ticketing system. It allows admins to set up user roles, manage departments, configure email settings, customize ticket fields, and generate reports. Essentially, it is used for system administration and configuration.

<img src="https://github.com/user-attachments/assets/3dab8a1d-cfc3-4c00-9a33-90ab6111715a" height="700" width="700" alt="Agent Panel"/>

### Agent Panel on osTicket
The **Agent Panel** is the interface used by support agents to handle incoming support tickets. Agents can view, respond to, and manage tickets assigned to them or their department. This panel provides tools for communication with customers, tracking ticket status, and collaborating with other agents.

### Key Differences
- **Purpose**: The Admin Panel is for system configuration and management, while the Agent Panel is for handling and responding to support tickets.
- **User Role**: The Admin Panel is accessed by administrators, whereas the Agent Panel is accessed by support agents.
- **Functionality**: Admins can customize settings and manage users, while agents focus on ticket resolution and customer interaction.

These distinctions help ensure that the system is both well-managed and responsive to customer needs.

<p>
  <img src="https://i.imgur.com/DJmEXEB.png" height="600" width="450" alt="Placeholder Image"/>
  <img src="https://i.imgur.com/DJmEXEB.png" height="600" width="450" alt="Placeholder Image"/>
</p>




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






