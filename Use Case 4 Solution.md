# Customer Service Team

## Managing Shared Mailboxes for Teams and Departments

The below steps are involved in creating, configuring, and managing shared mailboxes for teams and departments:

## 1. Creating a shared mailbox
Shared Mailboxes in Microsoft 365 are centralized mailboxes that multiple users can access and manage. It allows a team—such as customer service, HR, or IT support—to receive, read, and respond to emails from a common address (e.g., support@company.com) without requiring a separate license for each user accessing it.

## Steps to creating a shared mailbox for a *customer service team*:
- Sign in to the Microsoft 365 Admin Center
- In the left navigation pane, go to Teams & Groups > Shared Mailboxes
- Click on Add a shared mailbox
- Enter:
•	Name: Customer Service Support Mailbox
•	Email: Customerservice
- Click Save changes
- Go back to Teams & Groups > Shared Mailboxes (To see that the customer service support mailbox was created) 

## 2. Assigning members to a shared mailbox (Team Access)
Once a shared mailbox is created, the next critical step is assigning members who will manage it. These members act as the frontline team—responding to emails, tracking inquiries, and maintaining smooth communication. Assigning the right access roles ensures each team member has the correct level of interaction with the mailbox, whether it's reading, replying, or sending emails on behalf of the group.

## Steps to assigning members to the shared mailbox created for the *customer service team*:
- Click on the shared mailbox (customer service support mailbox)
- Under Members, click Edit
- Click Add Members (They will get Full Access & Send As permissions by default)
- Choose Users (Members) > Add (It saves automatically) 

## 3. Configuring Additional Permissions for the Customer Service Team
This involves setting the necessary permissions for members as opposed to the default permissions when members were added.

## Steps in Configuring Additional Permissions for the *Customer Service Team*:
- Sign in to the Exchange admin center (EAC) (This can also be done in the Microsoft 365 Admin Center)
- Navigate to Recipients > Mailboxes.
- In the list of mailboxes, select the shared mailbox (Customer Service Support Mailbox)
- On the flyout pane, Click the three dots (…) to edit “Send on Behalf” permission
- Click Send on Behalf > Add > Save > Confirm
- On the flyout pane, select Delegation
- Click “Edit” under Send As (To make changes to the Send As permission) > Confirm
- Click “Edit” under Read and Manage (Full Access) > Confirm


## PROJECT SUMMARY:
Implementing shared mailboxes for the customer service team enhanced communication efficiency, collaboration, and accountability. By creating a centralized mailbox in Exchange Online, team members could now respond to support inquiries from a unified address, maintaining consistent communication with clients. Permissions such as *Send As*, *Send on Behalf*, and *Full Access* were configured to ensure smooth operations and clear ownership. This setup not only streamlined internal workflow but also allowed real-time visibility into customer correspondence, thereby improving response times and service quality.

















