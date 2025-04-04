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


