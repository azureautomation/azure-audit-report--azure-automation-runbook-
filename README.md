Azure audit report (Azure automation runbook)
=============================================

            

Want to know about innovative and interesting ideas in Azure and automation? Check out my blog: https://manjunathrao.com/


 


The PowerShell script is an Azure automation runbook that pulls the below data and populates the data into a CSV file. The script then summarizes the data into an email's body and sends an email to the recipient with the CSV files as attachments.


 


If the Azure automation runbook is scheduled to run every day, you will get a summary/high-level view of what is happening in your environment to your email box. The email could be the first report any organization's high management would desire
 to look at. 


1. Count of De-allocated Azure virtual machines


2. Count of Running Azure virtual machines


3. Count of Stopped Azure virtual machines


4. Count of Azure virtual machines that do not have native backup configured (Azure Back up and Recovery service)


5. Count of Inbound Security rules that causes vulnerability


 


Email is sent via SendGrid service. You need to update the script with your SendGrid credentials.


 


You may choose a 'Free Tier' pricing for SendGrid. Below is documentation to create a SendGrid account:


https://docs.microsoft.com/en-us/azure/sendgrid-dotnet-how-to-send-email


 


If you would like me to add more data that would be useful as an Azure audit report, please let me know. 


Note: The script is an Azure Automation runbook. You have to run it from an Azure Automation account.


**Sample code:**


 

 

        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
