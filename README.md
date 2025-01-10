
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket. We will configure roles, departments, teams, agents, users, SLA's, and help topics. The configurations do not cover everything that can be done in osTicket but show a handful of things that model a typical ticketing system. Feel free to do more than what is on this tutorial.<br />
<h2>Prerequisites</h2>
<p>Install osTicket www.github.com/anakamura1/osticket-prereqs</p>
<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Configuration Steps</h2>

<table>
  <tr>
    <td>
      <img height="170%" width="170%" alt="Screenshot 2025-01-09 at 12 13 56 PM" src="https://github.com/user-attachments/assets/a317421d-f8a0-4cca-af5f-501cfeb7cf47" />
    </td>
    <td>
      <img height="80% width="80%" alt="Screenshot 2025-01-09 at 12 14 05 PM" src="https://github.com/user-attachments/assets/91cf7736-f7d6-4108-b2c0-c3d6b2b94024" />
    </td>
    </tr>
    </table>

</p>
<p>
  Begin making sure you are in the Admin panel. If the top right status says "Agent Panel" then we know we are in the Admin panel. 
</p>
<p>Configure a role by navigating to Agents -> Roles. We can name this role "Supreme Admin". In the permissions tab, select every permission for this role. Be sure to go through every permission tab for this role. Finish by "Add Role"
</p>
<br />

<P><img height="80%" width="80%" alt="Screenshot 2025-01-09 at 12 18 54 PM" src="https://github.com/user-attachments/assets/298e1c41-38de-4fb2-9491-789f1a1e6f32" />
</P>
<p>
  Configure departments by navigating to Agents -> Departments. Select Top Level Department and name the department System Administrators.
</p>
<br />

<p>
<img height="80%" width="80%" alt="Screenshot 2025-01-09 at 12 21 50 PM" src="https://github.com/user-attachments/assets/39965334-7138-4e52-97a8-c39122adb031" />
</p>
<p>
Configure teams by navigating to Agents -> Teams. We can name this team "Mobile Banking". After we create some agents, they can be added to this team.
</p>
<br />

<p>
  <table>
    <tr>
      <td>
          <img width="962" alt="Screenshot 2025-01-09 at 12 24 56 PM" src="https://github.com/user-attachments/assets/b04af488-fc77-4d58-b276-b85edc2afb4b" />
      </td>
      <td>
      <img width="957" alt="Screenshot 2025-01-09 at 12 25 23 PM" src="https://github.com/user-attachments/assets/8cddaac9-48dd-450e-a5bd-e4c86b0aeaea" />
      </td>
    </tr>
  </table>
</p>
<p>
  Configure a few agents by navigating to Agents -> Add New. We can create a new agent and set their login credentials by clicking "set password".
</p>
<p>We can give this agent a department and assign this agent the Supreme Admin role we created earlier. In the Permissions and Teams tab, we can give our agent all permissions and assign her to the "Mobile Banking" team.</p>
<br />

<table><tr>
  <td><img height="140%" width="140%" alt="Screenshot 2025-01-09 at 12 27 55 PM" src="https://github.com/user-attachments/assets/7414042f-a91f-46f0-9a5a-9ae6aa960742" />
</td>
  <td><img height="160%" width="160%" alt="Screenshot 2025-01-09 at 12 28 59 PM" src="https://github.com/user-attachments/assets/0d0c4c7a-e075-4950-a449-eaea902c5f11" />
</td>
</tr></table>
<p>
Configure another agent and assign this agent the Support role in the Access tab with All Access. Choose what permissions he can have in the Permissions tab. I recommend giving him permissions to at least work tickets for our Ticket Life Cycle Simulation project.</p>
<br />

<table>
  <tr>
    <td>
<img width="958" alt="Screenshot 2025-01-09 at 12 32 01 PM" src="https://github.com/user-attachments/assets/3673e93f-6ca5-4aac-94a5-35b0e76ad750" />
    </td>
    <td>
<img width="961" alt="Screenshot 2025-01-09 at 12 32 48 PM" src="https://github.com/user-attachments/assets/d9f075d4-edb5-4172-9080-852c41ac436d" />
    </td>
  </tr>
</table>
<p>
  Configure a few users by navigating to Agent Panel -> Users -> Add New. 
</p>
<br />

<table>
  <tr>
    <td><img width="959" alt="Screenshot 2025-01-09 at 12 34 31 PM" src="https://github.com/user-attachments/assets/fe2f73ed-660c-425d-871c-b20d639634fe" />
</td>
    <td>
      <img width="958" alt="Screenshot 2025-01-09 at 12 35 55 PM" src="https://github.com/user-attachments/assets/cb0ba52a-ff97-4c60-a1be-33eb87345c4c" />
    </td>
  </tr>
</table>
<p>
Configure SLA's by navigating to Manage -> SLA
</p>
  <p>
    Configure a few different SLAs with various schedules and grace periods. These will be used in our Ticket Life Cycle lab to determine the urgency of various tickets. 
  </p>
  <br>
  
<img height="80%" width="80%" alt="Screenshot 2025-01-09 at 12 41 08 PM" src="https://github.com/user-attachments/assets/424541a1-a478-4258-b481-1b0f9e9e418d" />
<p> Configure Help Topics by navigating to Manage -> Help Topics. Their priorities and various other items can be configured in the New ticket options tab.
</p>

<p>Several help topics can be created.</p>
  <p>
    <img height="80%" width="80%" alt="Screenshot 2025-01-09 at 12 48 32 PM" src="https://github.com/user-attachments/assets/7cbcf56e-496e-45a1-ab14-1dd33439d0a0" />

  </p>
  <P>A sample of various help topics.</P>

**This completes our configuration lab. See the Ticket Life Cycle Simulation lab next!**


