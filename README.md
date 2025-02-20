# Invitation Party Manager Website
This website allows the user to add parties and manage its invitations by sending them through email and recording its replies.
It is simple to manage the parties and verify who replied with YES or NO for the attendence.

The project contains a MIT license because is a simple software and does not contain any innovative logic. It still needs a lot of improvements and can be done by other contributors to make it better.
Given the simplicity, there is no need for legal complexity and contributors will have more flexibility to work on it.


## How to run the code
1. To run the code, it is necessary to install Visual Studio 2022, SQL Server 2022 (https://learn.microsoft.com/en-us/sql/database-engine/install-windows/install-sql-server-from-the-installation-wizard-setup?view=sql-server-ver16) and SQL Server Management Studio 20 (https://learn.microsoft.com/en-us/ssms/download-sql-server-management-studio-ssms).

2. Set the SQL Server with your SQL Server Management Studio using localhost. More details in https://learn.microsoft.com/en-us/ssms/quickstarts/ssms-connect-query-sql-server

3. On Visual Studio, make sure the NuGet Packages Microsoft.EntityFrameworkCore, Microsoft.EntityFrameworkCore.SqlServer and Microsoft.EntityFrameworkCore.Tools on version 7.0 to properly run with .NET 6.0. For details to install packages visit https://learn.microsoft.com/en-us/nuget/consume-packages/install-use-packages-visual-studio

4. Open the NuGet package console in Visual Studio under Tools> NuGet package Manager
On NuGet package console, run "Update-Database" to create the database on the server and wait for the process to be done.

5. Now you are ready to run it.

> [!TIP]
> If you want to select the browser you want to use when running the code, select the arrow down on the right side of the run button> Web Browser and select the desired browser.

![image](https://github.com/user-attachments/assets/48763285-7c14-408f-a7a9-2e462ae883d0)

## The Website
The main page is simple and gives you the option to see all the parties in database or already add one:
![image](https://github.com/user-attachments/assets/f91a7dea-4945-4bf9-81c3-dfddb7e47ea3)


By clicking on "parties" all parties saved in database will be displayed:
![image](https://github.com/user-attachments/assets/e3be303c-b21d-45bb-ad27-034c844787cb)


When clicking on "Manage" you have access to the invitations for the party.
When you create an invite, the initial status is "InvitationNotSent". 

Create as many invitations you desire then click "Send Invitation" and an invite will be sent to all the invites with status "InvitationNotSent".
The image below represents an invite created.
![image](https://github.com/user-attachments/assets/236cedba-d6a0-40a9-8ed7-24fda5e4274f)

The status available are:
* InvitationNotSent: invite was created
* InvitationSent: the email was sent
* RespondedYes: the guest replied YES
* RespondedNo: the guest replied NO

The invite sent through email will contain the name of the guest, the party name, location, date and a link to reply:
![image](https://github.com/user-attachments/assets/bb1a81f3-cc7e-409d-a6c3-e3e86b557141)

The link will give the option to reply YES or NO and according to the reply, the invite status will be changed in the website.
![image](https://github.com/user-attachments/assets/6571e9de-c559-4eb1-98be-ad22a9c520d5)




