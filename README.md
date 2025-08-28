![image](https://github.com/user-attachments/assets/825f97d3-91e6-4be2-8faa-86842daaa297)
<h1>Configuring a virtual machine and remote desktop (Azure)</h1>
This tutorial outlines the implementation of Azure Virtual Machines and remote desktop.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop


<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 



<h2>Deployment and Configuration Steps</h2>
<h2>CREATING VIRTUAL MACHINE</h2>


1. Visit Azure
- Go to azure.microsoft.com.

2. Sign Up for a Free Account
- Sign up for a free 30-day subscription.
- Create a username and password for your tenant.
- Access the portal anytime at portal.azure.com using your credentials.
![image](https://github.com/user-attachments/assets/cb1c6cb2-9142-47a5-92f1-f3a24c26ed3d)





3. Create a Resource Group
- In the search bar, type "Resource Groups" and click on "Create Resource Group".
![image](https://github.com/user-attachments/assets/3f413928-9fa7-4661-8fb4-c65553521eca)

- Enter a name for your resource group.
- Under "Resource Details," choose your desired region.
- Click "Review + Create." After validation, click "Create" to set up the resource group.
![image](https://github.com/user-attachments/assets/44c9f750-83e1-48e6-8442-4422aad740c0)




4. Create a Virtual Machine
- In the search bar, type "Virtual Machines."
![image](https://github.com/user-attachments/assets/219fc684-bb34-4651-8961-9461fa09ebe2)

- Click "Create," then select "Azure Virtual Machine."
![image](https://github.com/user-attachments/assets/6cbd1ff1-6262-4679-bced-63fb8c970814)

- In the creation form:
- Select your Azure Subscription and the Resource Group you just created.
- Name your Virtual Machine.
- Choose the same region as your resource group.
![image](https://github.com/user-attachments/assets/c1bbfc54-ca45-499f-b7ef-07c3a51ef923)

- Select your desired Operating System under "Image."(windows 10 pro)
- Pick the desired Size for your virtual CPU.(Standard D2s_v3 - 2 vcpus, 8 GiB memory)
![image](https://github.com/user-attachments/assets/5e2df3f8-aa05-4a8c-a2f5-f9b237ead954)


- Create a username and password for the Administrator account.
- Check the licensing box.
Click "Review + Create." After validation, click "Create." This may take a few minutes.
![image](https://github.com/user-attachments/assets/ab17b907-aada-4d4a-a698-1c53ad765778)


Congratulations on creating your Virtual Machine!

 
 <h2>Remote access</h2>


1. Access Your Virtual Machine
- In the search bar, type "Virtual Machines" or find it under the "Azure Services" tab.
- Click on the name of the VM you created to access the overview page.
[
](https://private-user-images.githubusercontent.com/183324257/372301928-219fc684-bb34-4651-8961-9461fa09ebe2.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3Mjc3NTI3OTIsIm5iZiI6MTcyNzc1MjQ5MiwicGF0aCI6Ii8xODMzMjQyNTcvMzcyMzAxOTI4LTIxOWZjNjg0LWJiMzQtNDY1MS04OTYxLTk0NjFmYTA5ZWJlMi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQxMDAxJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MTAwMVQwMzE0NTJaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT00ZGViN2RlYTY3YThlOTBkODk0MzhlNDVmMzc5YzQ2ZmU3Mjk2YmUwY2E0NjI4MjAzNTBmZDk3MDI0N2Y5ZmM3JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.UcvE2Wl1F2NfWeh9HIk9aCIC06HurUuxjZpz8-o1uiE)![image](https://github.com/user-attachments/assets/777c74f3-9d7f-4baa-b923-110d9519d51d)

- Note the Public IP Address displayed.
![image](https://github.com/user-attachments/assets/4f01d49b-e174-47f2-a966-7d9ce2a5e70e)





2. For Windows Users
- Open the Start menu and type "Remote Desktop."
- Paste or type the public IP address into the Remote Desktop Connection window.
![image](https://github.com/user-attachments/assets/591a6a83-79f6-411e-8ce2-3dc34ac4d329)

- Enter the username and password you created for the VM.
- If you receive a warning about security, click Yes to proceed.
- Your Virtual Machine should load; enter your username and password when prompted.


![image](https://github.com/user-attachments/assets/e3bc2421-98df-4395-836d-8582788db287)

- Connecting to Your VM


![image](https://github.com/user-attachments/assets/4860d276-db2c-4de3-a870-1e1ea34048b4)



3. For Mac Users
- Download "windows app" from the App Store (it's free).
![image](https://github.com/user-attachments/assets/5225a579-c0df-471d-a912-30c2bce1459b)


- Open the app and click the + sign to Add PC.
![image](https://github.com/user-attachments/assets/a950947a-cc2d-404c-bb54-a1df316fdf06)


- Enter the public IP address under "PC Name."
![image](https://github.com/user-attachments/assets/b9c7114d-9459-4ba6-abe1-da0ec58dc4ae)



- Under "Saved PC," enter the VM's username and password.
- Click continue.
![image](https://github.com/user-attachments/assets/2a52a822-9186-450c-adb5-cb7fe9ae0578)

4. Connecting to Your VM
![image](https://github.com/user-attachments/assets/6773ccfd-31b0-40eb-bd90-161b7e6e8820)


<h2>Deleting Your Virtual Machine</h2>

1. To delete your VM and associated resources:
- Go back to the Azure portal.
![image](https://github.com/user-attachments/assets/c72b1037-3cbe-4e31-822a-fe81319e2124)

- Navigate to your Resource Group.
- Delete the resource group and any related folders (e.g., NetworkWatcherRG).
(RG-network-activitie)
![image](https://github.com/user-attachments/assets/ff63b762-f0b5-46d9-955e-1d537c2d9119)


And that's it! You've successfully created, accessed, and deleted a Virtual Machine on Azure.
