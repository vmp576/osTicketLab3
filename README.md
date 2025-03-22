<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

# osTicket - Ticket Lifecycle Examples (Lab 3)

This project is the final osTicket lab, going over some example lifecycles for tickets. It will go over various SLA levels, comments, and various other configurations of a ticket.

## Environments and Technologies Used

- Completed osTicket Lab 2 Virtual Machine in VMware

## Operating Systems Used
 - Windows 10 (22H2)

## Project Walk-Through/Lifecycle Stages
### Intake

To start, go to the end user site of osTicket through this link: http://localhost/osTicket and **Create a New Ticket**

<img src="https://i.imgur.com/xgxL9b0.png" height="70%" width="70%"/>

Create a ticket with the following properties:

- Email: karen@user.com
- Full Name: Karen
- Help Topic: Report a Problem
- Issue Summary: entire mobile/online banking system is down
- Details: My employees are reporting that users can no longer access their online banking portal. The ones who can occasionally access it cannot log in.

<img src="https://i.imgur.com/04HzrD6.png" height="70%" width="70%"/>

### Assignment and Communication

Now, sign into the agent [osTicket](http://localhost/osTicket/scp/login.php) link as John (Username: johndoe. Password: Password123!). If you’re logged in as any other user, log out. Here, you can observe the newly created ticket.

<img src="https://i.imgur.com/SzjzGQh.png" height="70%" width="70%"/>

As John, observe the ticket's properties (Priority, Department, SLA, Assigned To). Because John was configured as a read-only agent, pretend that John has communicated with their superiors about the ticket and that the ticket will be escalated. Add an internal note about the escalation and log in with Jane after (Username: janedoe. Password: Password123!).

<img src="https://i.imgur.com/QEc4luM.png" height="70%" width="70%"/>

### Working the Issue and Resolution

After logging into Jane’s account, access the mobile banking ticket. Several discrepancies with the ticket need to be fixed while working on the ticket. Firstly, the incorrect priority and help topic are assigned. It is originally listed as a “Normal” level priority. However, critical business outages are a “High” priority. Adjust the ticket by:

- Set Priority → High
- Assigned To → Online Banking Team
- Help Topic → Business Critical Outage
- SLA Plan → Sev-A

After making adjustments, make a “resolved” reply such as the reply below to complete the ticket.

<img src="https://i.imgur.com/AibrXCz.png" height="70%" width="70%"/>

After completing the ticket above, you should know how to use the osTicket ticketing system and should be able to create, adjust, and resolve your own tickets. The following is another scenario that can be used for extra practice.

**End User Ticket**

CFO’s laptop will no longer turn on

**Help Desk Agent Response (Adjust the following fields)**

- Priority (Normal)
- Department (Support)
- SLA (Sev-B)
- Assigned To (Tier I Support)
