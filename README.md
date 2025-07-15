# osTicket-Post-Installation-Configuration

*This lab will outline the post-install configuration of the open source help desk ticketing system osTicket prior to working mock-tickets in the next lab.*

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

-  [osTicket Prereqisites lab](https://github.com/EddieJIV/osticket-prereqs) 

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
- Click, "Add New Role".

<p>
  <img src="https://github.com/user-attachments/assets/b3800554-2323-43d2-91af-a30daac1bc5e" height="600" width="450" alt="Supreme Admin"/>
  <img src="https://github.com/user-attachments/assets/e8caa6c8-d508-405e-a8b7-3abbb195fe5e" height="600" width="450" alt="Permissions"/>
</p>

- Give the title of this new role "Supreme Admin"
- Move on to the Permissions tab, and check every box under the tickets, tasks, and knowledgebase sections. Effectively giving this new Supreme Admin role full access to do absolutely everything.
- Click, Add Role.

## 3. Department Configuartion
*To organize support agents into specific groups based on their roles, expertise, or the types of tickets they handle.*

<img src="https://github.com/user-attachments/assets/697d6675-9e7b-4209-9ce5-4060a3878942" height="700" width="700" alt="Departments"/>

- Navigate to the Department heading.
  - Admin Panel > Agents > Departments
- Click, "Add New Department". 

<img src="https://github.com/user-attachments/assets/f7579cc8-0379-47be-a441-51ed40c68e09" height="700" width="700" alt="SysAdmins Create"/>

- Since we havent set up any SLA's or created agents yet, we are simply going to make a new department called "SysAdmins" and make it a Top-Level Department.
- Once you see that the parent is Top-Level Department, and the name is SysAdmins, you can simply click create.

<img width="700" height="700" alt="Housekeeping" src="https://github.com/user-attachments/assets/0e60c5e4-763b-4b78-9dca-122c57d570fd" />

- We additionally need to delete the preset maintenance department. We will use and create our own departments to work in for the sake of this lab and deleteing this preset will allow us to do so without any hitches.
  - To delete, check the box next to maintenance, click on the button labeled "More", then delete.


## 4. Team Configuration
*To group agents into collaborative units for more efficient ticket management.*

<img src="https://github.com/user-attachments/assets/ff046049-e035-4469-8680-c7e589f61b07" height="700" width="700" alt="Teams (new)"/>

- Navigate to the Teams heading.
  - Admin Panel > Agents > Teams
- Click, "Add New Team".

<img src="https://github.com/user-attachments/assets/07c4e859-7025-4c4f-bdb4-c0f21e1420f3" height="700" width="700" alt="Online Banking"/>

- We are going to create a new team called "Online Banking"
- Since we have not made any agents yet you do not have to worry about the members tab or assigning a team lead, we can just simply click create from here.

## 5. Agent & User Configuration
*To manage the support agents who will handle incoming tickets & the end-users or customers who submit support tickets.*

<img src="https://github.com/user-attachments/assets/ae7ca2c0-6cc0-4f8c-a724-ec0c3dfe7254" height="700" width="700" alt="Agents (add new)"/>

- Now, we are going to create and add two new workers (agents) and create agent accounts for them.
  - From the Admin Panel navigate to Agents > Agents
- Click "Add New Agent". We are going to add two new agents, "Jane" and "John"
<img src="https://github.com/user-attachments/assets/438afed5-1c4b-4b3c-b023-aeb263e28326" height="700" width="700" alt="Jane"/>

- Add our first agent to osTicket, Jane.
  - note that the email jane@gmail.com is (obviously) fake and can still be entered.
- Simply make Jane's username, "Jane".
- Once you've entered Jane's username, click "Set Password".

<img src="https://github.com/user-attachments/assets/294127ef-0f97-4eab-8a82-2c9dbaf1a43a" height="700" width="700" alt="Password1"/>

- Upon clicking "Set Password", uncheck the box saying to send the agent a password reset email.
- Also, uncheck the box saying, "Require password change at next login"
- For simplicity and the sake of the lab, because it is easy to remember, make Janes password, "Password1" then click, "Set".
  - It would be beneficial to write down Jane's (and John's when we make his) account username and password since we will be loggin into their accounts to work tickets.
- Before clicking create, find the Access tab and navigate there for the next step. 

<img src="https://github.com/user-attachments/assets/b766262e-4add-4412-a55f-ee1c9167308a" height="700" width="700" alt="Jane's Access"/>

- We are going to make Jane a part of the SysAdmins Department and we are also going to make her a Supreme Admin, giving her access to everything.
- Next, we can skip over the permissions tab and move on to the Teams tab.

<img src="https://github.com/user-attachments/assets/d6580bf6-06eb-4e7c-8b36-507edbcfe99c" height="700" width="700" alt="Jane's Team"/>

- Make Jane a part of the Online Banking team.
- Click "Create".

<img src="https://github.com/user-attachments/assets/a0d8fee2-62db-4cc2-bf60-1587d8803f8e" height="700" width="700" alt="Agent Home-Add John"/>

- Now, back at the home page of the Agent panel we can see our newly added agent, Ms. Jane Doe.
- We are also going to click "Add New Agent" once more and add John.

<img src="https://github.com/user-attachments/assets/82d2692a-0c04-4a33-84bb-12435af26ed2" height="700" width="700" alt="John Doe"/>

- Enter Jon Doe's name and fake email address.
- Make his username "John".
- Click "Set Password".
  - Uncheck the "Send the agent a password reset email" box
  - Make the password, "Password1".
  - Uncheck the require password change box
  - Click "Set".
- Before clicking create we are going to move to the Access tab.

<img width="700" height="700" alt="Johns Access" src="https://github.com/user-attachments/assets/4a063256-c368-4947-867e-a53337ea2a5f" />

- For the sake of this lab we are going to make him a part of the Support Department and give him "All Access"
- Leave Permission and Teams alone, and click "Create".

<img src="https://github.com/user-attachments/assets/bb083868-a7e6-42be-96b7-152481d38787" height="700" width="700" alt="Add User"/>

- For the next step, we are going to add an end-user, Karen, to our system.
- In order to do so, we need to navigate to the Agent Panel.
  - This can be found in the top right corner of the web page next to the Welcome text.
- Navigate to the User Directory
  - Agent Panel > Users > User Directory
- Click, "Add User."

<img src="https://github.com/user-attachments/assets/b3412703-c44f-4b80-a0ca-51960de3109d" height="700" width="700" alt="Add Karen"/>

- Add Karen to the user database.
  - Again, enter or make up a fake email address for our new client.
- Click, "Add User".

## 6. SLA Configuration
*To define and manage service level agreements for ticket response and resolution times.*

<img src="https://github.com/user-attachments/assets/52e6ccca-3ce9-4986-b78e-d1dbdfde031d" height="700" width="700" alt="SLA NAV"/>

- First, navigate back to the Admin Panel.
- Then, under the "Manage" tab, Click on "SLA".
- We are going to configure 3 SLA's.
  - Sev-A, Sev-B, and Sev-C
- Each severity level (Sev-A, Sev-B, Sev-C) has distinct grace periods and schedules, which are crucial for prioritizing support responses based on the urgency of the issues reported.
- Click, "Add New SLA Plan" to navigate to the next step.

<img src="https://github.com/user-attachments/assets/e1a99f68-34dc-4a17-9c40-d49f626764eb" height="700" width="700" alt="Sev-A"/>

- For the name, as mentioned, we are going to put Sev-A.
- With a Grace period of 1 hour
- And a Schedule of 24/7.
- Click, "Add Plan".
  
Sev-A represents the highest priority level, typically reserved for critical issues that severely impact business operations or cause significant disruption.

- Click, "Add New SLA Plan" to navigate to the next step.

<img src="https://github.com/user-attachments/assets/e700863a-3af7-4fdc-99e1-646927aedd8d" height="700" width="700" alt="Sev-B"/>

- Now, we are going to add Sev-B
- Give Sev-B a grace period of 4 hours.
- And a Schedule of 24/7.
- Click, "Add Plan".

Sev-B is for high-priority issues that need timely resolution but are not as urgent as Sev-A. These issues may affect a significant number of users or critical functions but do not cause immediate disruption.

- Click, "Add New SLA Plan" to navigate to the next step one last time.

<img src="https://github.com/user-attachments/assets/2b2c8e42-aa07-4160-aaa4-d9be7aba0ce7" height="700" width="700" alt="Sev-C"/>

- Finally, we are going to add Sev-C.
- Give Sev-C a grace period of 8 hours
- And a schedule of normal business hours.
- Click, "Add Plan".

Sev-C will be designated for lower-priority issues that do not significantly impact business operations or user experience and their resoultion times will be limited to normal business hours.

## 7. Help Topic Configuration
*To create and manage predefined topics that categorize support tickets based on common issues or inquiries.*

<img src="https://github.com/user-attachments/assets/8c2312f8-5c63-4aba-b9b3-53ffb5c02889" height="700" width="700" alt="Help Topic Home Page"/>

- Finally, we are going to set up help topics for when users create tickets.
- In order to do so, navigate over to "Help Tpoics" still under the manage tab.

We are going to create 5 new Help Tpoics for our "users" to help organize support requests and attempt to facilitate more efficient communication between users and support agents.

- Click, "Add New Help Topic" to begin.

<img src="https://github.com/user-attachments/assets/93e03b47-f50b-442d-a193-132e5bd9f83e" height="700" width="700" alt="HT 1"/>

- For our first Help Topic, we are going to name it, "Business Critical Outage".
- With a parent topic of, "Report a Problem".
- Following this we can simply click "Add Topic" and return to the Help Topics page.

<img src="https://github.com/user-attachments/assets/0753e766-885b-4c35-a1c2-b2bc211a36cf" height="700" width="700" alt="HT 2"/>

- For our second Help Topic, we are going to name it, "Personal Computer Issues".
- With a parent topic of, "Report a Problem".
- Following this we can simply click "Add Topic" and return to the Help Topics page.

<img src="https://github.com/user-attachments/assets/416af425-91ad-417a-872a-9679e1b5bfb3" height="700" width="700" alt="HT 3"/>

- For our third Help Topic, we are going to name it, "Equipment Request".
- With a parent topic of, "General Inquiry".
- Following this we can simply click "Add Topic" and return to the Help Topics page.

<img src="https://github.com/user-attachments/assets/ee36dedf-19ce-4a1b-8d5b-d374da381923" height="700" width="700" alt="HT 4"/>

- For our fourth Help Topic, we are going to add every end-users favortie request, the infamous, "Password Reset".
- With a parent topic of, "Report a Problem/ Access Issue".
- Following this we can simply click "Add Topic" and return to the Help Topics page.

<img src="https://github.com/user-attachments/assets/dec69e57-81c3-4699-b47f-e2f414836d6a" height="700" width="700" alt="HT 5"/>

- For our fifth and final Help Topic, we are going to name it, "Other".
- With a parent topic of, "General Inquiry".
- Following this we can simply click "Add Topic".
  
---

This effectively concludes my osTicket Post-Installation-Configuration lab! 

I hope you'll join me in my third and final lab in this osTicket lab series wherein we will finally work on some common help desk tickets within osTicket.







