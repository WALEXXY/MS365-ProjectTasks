# Micadak Investments

## Setting Up Outbound Email Routing and Transport Rules

The below steps are involved in preventing users from sending credit card information via email:

## 1. Configure a Data Loss Prevention (DLP Policy)
The Data Loss Prevention (DLP) policy created in Microsoft Purview is designed to detect and block emails containing credit card numbers in Exchange Online. It helps protect sensitive financial information from being accidentally or maliciously sent outside the organization. When a user attempts to send such information, the DLP policy automatically blocks the email and displays a policy tip, informing the sender about the violation and encouraging secure data handling practices. This ensures compliance with data protection standards likePayment Card Industry Data Security Standard (PCI-DSS) and enhances the organization’s overall information security posture.

## Steps to configure a data loss prevention policy for *Micadak Investments*:
- Go to Microsoft Purview Portal (purview.microsoft.com)
- Navigate to Data loss prevention > Policies > Create policy
- Choose ‘Custom Policy’ > Next
- Name your DLP policy > Next
- Assign Admin units > Next
- Choose Location: Exchange email > Next
- Define policy settings > Next
- Create Rules:
Add Credit Card Number as a condition
Action: Block message with policy tip
Add policy tips to educate users on safe data practices
- Customize advanced DLP rules > Next
- Set Policy mode > Next 
- Click Submit > Done

## 2. Add a Disclaimer to Outgoing Emails
This is useful for legal or informational messages like:
“This email may contain confidential information intended only for the recipient”

## Steps to adding a disclaimer to outgoing emails for *Micadak Investments*:
-	Go to Microsoft Exchange Admin Center (EAC) (admin.exchange.microsoft.com)
-	In the left menu, click on Mail flow > Rules
-	Click ‘+ Add a rule’ > Select ‘Create a new rule’
-	Set rule conditions
Name your rule (Add Disclaimer to all external emails)
Under ‘Apply this rule if’: Choose The recipient is external/internal > Select ‘Outside the organization’
Under ‘Do the following’: Choose Apply a disclaimer to the message > append a disclaimer
(Enter your disclaimer message - This email may contain confidential information intended only for the recipient) 
Choose fallback action: e.g., Wrap or Ignore
-	Set rule settings > Next > Done
-	click on Mail flow > Rules > Click on the newly created rule (Add Disclaimer to all external emails)
-	Click on ‘Disabled’ to enable the rule

## 3. Preventing Auto-Forwarding of Emails
Auto-forwarding can be a data leakage risk, so this rule blocks users from forwarding emails externally.

## Steps in preventing auto-forwarding of emails for *Micadak Investments*
-	Go to Microsoft Exchange Admin Center (EAC) (admin.exchange.microsoft.com)
-	In the left menu, click on Mail flow > Rules
-	Click ‘+ Add a rule’ > Select ‘Create a new rule’
-	Set rule conditions
Name your rule (Block Auto-Forwarding)
Under ‘Apply this rule if’: Choose ‘The Message properties’ > Select ‘include the message type’ – Choose ‘Auto-Forward’ as the message type
Under ‘Do the following’: Select ‘Block the message’ > Select ‘Reject the message and include an explanation’
(Enter a suitable explanation - Auto-forwarding to external recipients is not permitted) 
-	Set rule settings > Next 
-	Click ‘Finish’ after reviewing > ‘Done’
-	click on Mail flow > Rules > Click on the newly created rule (Block Auto-Forwarding)
-	Click on ‘Disabled’ to enable the rule
-	

PROJECT SUMMARY
To strengthen data security and ensure regulatory compliance, Micadak Investments initiated a project to prevent employees from sending emails containing credit card numbers. The primary objective was to mitigate the risk of accidental data exposure and meet data protection standards like PCI-DSS.
Using Microsoft Purview’s Data Loss Prevention (DLP) capabilities, we implemented a custom DLP policy targeting Exchange Online. This policy automatically detects the presence of credit card information and blocks outbound emails containing such data. Additionally, we configured policy tips to educate users about secure communication practices in real time.
To supplement the DLP strategy, we leveraged Mail Flow Rules in Exchange Online to:
•	Add email disclaimers for compliance and legal transparency,
•	Prevent auto-forwarding of emails to unauthorized external recipients.
This multi-layered approach provided Micadak Investments with a comprehensive email security framework, safeguarding sensitive financial data and reinforcing user awareness. It also helped position the organization to comply with industry regulations while maintaining seamless email communication.


