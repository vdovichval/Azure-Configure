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

![image](https://github.com/user-attachments/assets/d5a9425e-3cbc-4c8a-912d-2f26dd563064)






3. Create a Resource Group
- In the search bar, type "Resource Groups" and click on "Create Resource Group".

![image](https://github.com/user-attachments/assets/271e2e09-2af2-4348-9e7c-bd864858e460)



- Enter a name for your resource group.
- Under "Resource Details," choose your desired region.
- Click "Review + Create." After validation, click "Create" to set up the resource group.

![image](https://github.com/user-attachments/assets/c71578ab-49a2-4bf7-b7fa-a68b13d416b2)






4. Create a Virtual Machine
- In the search bar, type "Virtual Machines."

![image](https://github.com/user-attachments/assets/8d8e2657-b8b0-42d8-8e34-d7a850964cf6)


- Click "Create," then select "Azure Virtual Machine."

![5](https://github.com/user-attachments/assets/bd05f239-83fa-4165-9adc-d0429c30634f)


- In the creation form:
- Select your Azure Subscription and the Resource Group you just created.
- Name your Virtual Machine.
- Choose the same region as your resource group.
  
![6](https://github.com/user-attachments/assets/2e1dd41a-a87b-4307-933f-9a1b240ddddb)


- Select your desired Operating System under "Image."(windows 10 pro)
- Pick the desired Size for your virtual CPU.(Standard D2s_v3 - 2 vcpus, 8 GiB memory)
  
![7](https://github.com/user-attachments/assets/b507f7c0-020c-4422-af36-13ae0d1c48c1)


- Create a username and password for the Administrator account.
- Check the licensing box.
Click "Review + Create." After validation, click "Create." This may take a few minutes.

![8](https://github.com/user-attachments/assets/2ffc211a-3fd1-43a7-ae75-43f9858e5832)


Congratulations on creating your Virtual Machine!

 
 <h2>Remote access</h2>


1. Access Your Virtual Machine
- In the search bar, type "Virtual Machines" or find it under the "Azure Services" tab.
- Click on the name of the VM you created to access the overview page.
![2](https://github.com/user-attachments/assets/debace6b-08b1-49f4-b7d1-de67d03322cb)


- Note the Public IP Address displayed.
  
![9](https://github.com/user-attachments/assets/4723087e-a17f-450f-8cf2-b74019effc1c)






2. For Windows Users
- Open the Start menu and type "Remote Desktop."
- Paste or type the public IP address into the Remote Desktop Connection window.
  
![10](https://github.com/user-attachments/assets/14bbbfc9-e6df-4674-b9ea-b772c4081022)

- Enter the username and password you created for the VM.
- If you receive a warning about security, click Yes to proceed.
- Your Virtual Machine should load; enter your username and password when prompted.

![11](https://github.com/user-attachments/assets/b4607231-a43a-4acb-836e-499a51db01e6)


- Connecting to Your VM

![12](https://github.com/user-attachments/assets/38d529ff-9c4d-46cc-acf5-cd442e1f288e)





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
![13](https://github.com/user-attachments/assets/0bef72ac-61eb-40ff-9414-b9d3cf3beb6b)


- Navigate to your Resource Group.
- Delete the resource group and any related folders (e.g., NetworkWatcherRG).
(RG-network-activitie)

![14](https://github.com/user-attachments/assets/09626d47-bc95-4581-9d27-423edfe9b2e6)


And that's it! You've successfully created, accessed, and deleted a Virtual Machine on Azure.
