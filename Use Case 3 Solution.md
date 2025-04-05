# Sholz Financials

## Implementing Email Retention and Archiving Policies in Microsoft 365

The below steps are involved in implementing Email Retention and Archiving Policies:

## 1. Configuring Retention Policies in Microsoft Purview for *Sholz Financials*
Retention policies automatically store and protect emails for a specified duration, preventing deletion before the retention period ends.

## Steps to Configure Retention Policies in Microsoft Purview for *Sholz Financials*:
- Sign in to the Microsoft Purview portal
- Navigate to Solutions > Data Lifecycle Management
- Click Policies > Retention Policies > New Retention Policy
- Set Policy Name > Click Next.
- Set Policy Type > Click Next.
- Set Locations (Exchange Mailboxes) > Click Next
- Set Retention Settings > Click Next.
- Review the policy and confirm settings.
- Click Submit to create retention policy.
- Click Done
- Go back to Solutions > Data Lifecycle Management > Policies > Retention Policies (To see the policy newly created)

## 2. Enabling Archiving in Exchange Online
Archiving moves older emails to a separate mailbox instead of deleting them.

## Steps to enable archiving in Exchange Online for *Sholz Financials*:
- Sign in to the Exchange admin center (EAC) 
- Navigate to Recipients > Mailboxes.
- In the list of mailboxes, select the user mailbox/shared mailbox (Sholz Financials) 
- On the flyout pane, select Others > Manage mailbox archive:
- On the Manage mailbox archive pane, Enable ‘Mailbox archive status’ > Save.
- Go back to Recipients > Mailboxes (To see that Archive status for Sholz Financials is now active)

## 3. Apply Sensitivity Labels in Microsoft Purview to Archived Emails for *Sholz Financials*
Sensitivity Labels in Microsoft Purview classify and encrypt sensitive emails automatically.

## Steps to apply and publish sensitivity labels in Microsoft Purview to archived emails for *Sholz Financials*:
- Sign in to the Microsoft Purview portal
- Navigate to Solutions > Information Protection > Sensitivity Labels
- Click on ‘Create a label’ > Set Label details > Next
- Set Scope > Next
- Set Items (Access Control, Content Marking, Auto labeling for files and emails) > Next
- Define protection settings for groups & sites > Next
- Review & confirm the settings > Create label
- Go back to Sensitivity Labels to see the created label
- Click on the newly created label (SholzFinancials-Confidential) > Publish label > Next
- Select Users and Groups > Done > Next
- Set policy settings (Documents, Emails, Meetings, Fabric & Power BI) > Next
- Set Policy Name > Next
- Review & Confirm policy settings > Submit > Done

## 4. Enabling Litigation Hold for a User Mailbox
Litigation Hold ensures that emails and other mailbox items are preserved indefinitely or for a specified period, even if a user tries to delete them. This is crucial for compliance investigations, legal disputes, or regulatory audits.

## Steps to enable Litigation Hold for a User Mailbox for *Sholz Financials*:
- Sign in to the Exchange admin center (EAC) 
- Navigate to Recipients > Mailboxes.
- In the list of mailboxes, select the user mailbox/shared mailbox (Sholz Financials) 
- On the flyout pane, select Others > Manage litigation hold
- On the Manage litigation hold pane, enable ‘litigation hold’ (This brings out dialog boxes to be filled such as ‘Hold Duration’ and ‘Reason for the hold’ which are to be filled)
- Click Save to apply changes

 


