# Microsoft-Entra-Data-Protection-Access-Control
Description

In Today's Technology Landscape the importance of Data Protection, Access Control and Authentication are a top priority for organizations, who and for how long A current Employee, or Third party Collaborator have access to your Compnay data is an important topic that should always be monitored within the Organization, Making sure Right Controls are in place, and
you also want to ensure your Customers that there information is safe with you're organization, 


In this Lab I enabled Dynamic Data Masking For My SQL database lab, which is Azure SQL Database is a security feature that limits sensitive data exposure by masking it to non-privileged users. It helps prevent unauthorized access to sensitive data by displaying a masked version of the data to users who do not have the necessary permissions to view the unmasked data.
How It Works: DDM modifies the output of a query to hide sensitive information while still allowing non-privileged users to access the data. For example, Customers Email might be shown as XXX-XXX-.com instead of the full email address.
Use Cases: Protecting sensitive data such as personally identifiable information (PII), financial data, or any other critical information that should not be fully exposed to all users.

Also generated a Shared Access signature For storage account created for lab at the subscription level, and Blob level the key benifits of an SAS (Shared Access Signature)
it grants a time based access to Microsft Entra Resources, For a Specific amount of time could be little as a few days or up to a year, For a third party to accoumplish a task, could
be an Auditor that may want to Access your Environment To Review Policies, Or Application Developer from outside source, Granting temporary access to storage resources, enabling secure data sharing, and integrating storage access in applications without exposing sensitive credentials. 

<h1>Utilities Used</h1>

Azure SQL Database

Azure Storage Accounts

Dynamic Data Masking (DDM)

Shared Access Signatures (SAS)

<h1>Envrionments Used</h1>

Microsoft Entra

<h1>Program Walkthrough</h1> 
Enabling Dynamic Data Masking

![dynamic data masking](https://github.com/user-attachments/assets/2e0256a0-5ca3-4707-8a7c-1c1e1855c9fa)


Signed into SQL Database on my Admin Account Dynamic Data Masking is only for Non-Priveledge users has no effect on the Admin as you see Email addresses are still visible

![Datamasking-Admin Account](https://github.com/user-attachments/assets/fe5cc55b-1bf2-474c-8220-be80269e1547)

Created A non-priveledge user, now you can see the Email addresses are not visible

![image](https://github.com/user-attachments/assets/ebe6011f-6f63-4c7d-a7f3-12ed14442b38)


Creating SAS (Shared Access Signature) For Blob Storage similiar to file explorer for regular Windows OS Sytems store files and docments, only set for a day, you can allow only 
Certain IP addresses also Can use Https or Http Protocol.

![SASBLOB](https://github.com/user-attachments/assets/8f9aefa7-af86-436f-9f18-5351b3021ab7)


Shared Access Signature At Storage Account Level With List and Read Permission

![SASStoragelevel](https://github.com/user-attachments/assets/41a202cc-a305-4cd8-aa13-a12e0d6de6f9)


Azure Storage Explorer trying to upload Documents, but because only Read and list permissions was given request Failed

![SASuploadfailed](https://github.com/user-attachments/assets/93f240ac-1498-4e1a-8bd2-965ef344f83f)

<h1>Summary</h1>

In this lab wanted to really focus on the importance of implementing strong data protection and access control measures, ensuring that sensitive information is adequately protected and that temporary access is managed securely.










