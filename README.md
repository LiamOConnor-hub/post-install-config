<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Allow anyone to create tickets
- Configure Agents (workers)
- Configure Users (customers)
- Configure SLA
- Configure Help Topics (For when users create a ticket)

<h2>Configuration Steps</h2>

<p>
The first step after installing osTicket is to configure the roles, departments, and teams. Roles determine the specific permissions that agents will have, such as managing tickets or modifying system settings. Departments organize the ticket flow into categories like IT Support, Human Resources, or Customer Service, ensuring that requests go to the right place. Teams can then be created to group agents across departments, allowing specialized groups of workers to handle certain issues more effectively. Together, these configurations establish the structure of your support system.
</p>
<br />

<p>
The next step is to configure access for both agents and users. Agents are the workers who handle tickets, and each one needs to be assigned roles and departments so they can carry out their responsibilities. Users, or customers, are the people submitting tickets, and the system can be set up to automatically create user accounts when tickets are submitted. Additionally, settings can be adjusted to allow anyone to create a ticket without needing to log in, which makes the support system more accessible and user-friendly.
</p>
<br />

<p>
Finally, service expectations and support categories should be set up through SLA plans and help topics. SLA (Service Level Agreements) define the required response and resolution times for tickets, ensuring that issues are handled promptly and consistently. Help topics act as categories that users select when submitting a ticket, such as password resets, hardware issues, or billing problems. These topics help with ticket routing, prioritization, and efficiency in resolving issues. By completing this step, the support system becomes both organized and responsive to user needs.</p>

<h2>Configuration Step by Step</h2>

Configure Roles (for grouping permissions)
- Admin Panel -> Agents -> Roles
- Supreme Admin

Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
- Admin Panel -> Agents -> Departments
- SysAdmins

Configure Teams
- Admin Panel -> Agents -> Teams (Pull Agents from different Departments)
- Online Banking

Allow anyone to create tickets
- Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)
- Registration Required: Require registration and login to create tickets 

Configure Agents (workers)
- Admin Panel -> Agents -> Add New
- Jane (Dept: SysAdmins)
- John (Dept: Support)

Configure Users (customers)
- Agent Panel -> Users -> Add New
- Karen
- Ken

Configure SLA
- Admin Panel -> Manage -> SLA
- Sev-A (Grace Period: 1 hour, Schedule: 24/7)
- Sev-B (Grace Period: 4 hours, Schedule: 24/7)
- Sev-C (Grace Period: 8 hours, Business Hours)

Configure Help Topics (For when users create a ticket)
- Admin Panel -> Manage -> Help Topics
- Business Critical Outage
- Personal Computer Issues
- Equipment Request
- Password Reset
- Other

<br />
