<img width="1000" height="250" alt="microsoft-azure" src="https://github.com/user-attachments/assets/86e9ccf8-1383-49a6-a2fe-68b03806d5df" />

# Azure Windows VM Deployment Lab
Azure lab demonstrating the deployment and basic administration of a Windows virtual machine.

<h2>Environments and Technologies Used</h2>

- Azure Resource Group
- Microsoft Azure (Virtual Machines/Compute)
- Azure Virtual Network/Subnet
- Remote Desktop

<h2>Operating Systems Used </h2>

- Apple Mac OS (Host Machine)
- Windows 11 Pro </b> (25H2 ) (Virtual Machine)

<h2> Configuration Steps </h2>

- Step 1 - Create a Resource Group
- Step 2 - Create Windows 11 Pro VM within Resource Group
- Step 3 - Use Remote Desktop to test Windows VM functionality

<h2>Configuration Process</h2>

<img width="1554" height="670" alt="Creating azure resource group" src="https://github.com/user-attachments/assets/f3fd26fc-61e0-4d05-9eb0-681d0ad91f1b" />
</p>
<p>
When signing up for an Azure subscription, we’ll begin by searching for “Resource groups” in the Azure Portal search bar. Once “Resource groups” appears in the search bar, click on it and click create.
In the screenshot above, the details of the Resource group are as follows:

- Subscription: This refers to the Azure account or billing plan you select to pay for and manage the resources within your Resource Group.

- Resource Group Name: This is the unique name you assign to your Resource Group to identify and organize your resources.

- Region: This indicates the geographic location where Azure hosts your resources. Once filled in, click “Review + Create.”  
</p>
<br />
<p>
<img width="2112" height="548" alt="azure resource group created" src="https://github.com/user-attachments/assets/a0252b20-39c8-4934-8660-b66859006614" />
</p>
<p>
Microsoft Azure resource group has now been created and ready for use.

<h2> Deployment of Windows 11 Pro VM within Resource Group </h2>

<p>
<img width="1235" height="794" alt="3_create-vm" src="https://github.com/user-attachments/assets/67d83589-e0f2-4ed4-af24-3d0f7994cd3f" />
<p>
Now, let’s begin by searching for “Virtual Machines” in the Azure Portal search bar. Once “Virtual Machines” appears in the search bar, click on it under the “Services” section and then click “Create.” As shown in the screenshot above.
</p>
<img width="2554" height="1243" alt="Screenshot 2026-09-02 at 10 23 10 PM" src="https://github.com/user-attachments/assets/02b2b537-73dd-4621-aa50-3802a7b6f39f" />
</p>
Now, you will land on this page, as depicted in the screenshot above.</p>

- On this page, you can select a Microsoft Azure subscription and resource group. You can also give your virtual machine a name and choose the region where you’d like it to be hosted. You can choose from various operating systems like Windows and Linux, and select the size of your virtual machine, including RAM and storage capacity.
<img width="891" height="715" alt="Screenshot 2026-09-07 at 3 28 36 PM" src="https://github.com/user-attachments/assets/4dba7237-948d-4fc8-a751-952b782c075b" />

- On the same page, scroll down and fill in a user account name and password for the virtual machine and enable RDP (Remote Desktop Protocol) (3389), as this is what will allow you to remotely access the VM.

- If you don't select the option confirming an eligible Windows 10/11 license with multi-tenant hosting rights, Azure blocks the VM creation because it requires proof that you have a valid license to run Windows in a shared cloud environment. Select the checkbox and click "Next: Disks"
  <img width="1222" height="838" alt="9_disks" src="https://github.com/user-attachments/assets/5f7e0ddb-2979-4632-8e2f-a6fc629ff367" />
<h2> Click "Next: Networking" to move into the Networking section of the VM creation </h2>
<img width="2554" height="1243" alt="Screenshot 2026-09-02 at 10 26 43 PM" src="https://github.com/user-attachments/assets/cad19d2b-22bd-4200-9fb6-7017cc28a74f" />

- To rename a virtual network in Azure, click on “Edit virtual network” under “Virtual Network.”

-  Having virtual machines (VMs) on the same virtual network enables them to communicate swiftly and securely with minimal latency, as they reside within the same isolated network environment. This simplifies the setup for tasks such as testing or data sharing between VMs, eliminating the need for intricate routing or public internet access. Next, click on "Review + Create" to be taken to the VM summary page. 
 <img width="749" height="646" alt="Screenshot 2026-09-02 at 10 26 43 PM 2" src="https://github.com/user-attachments/assets/a8e9534d-89b9-4283-83ab-421c352a4045" />
 <img width="1017" height="584" alt="12_create-vm" src="https://github.com/user-attachments/assets/55c606b3-1faa-44d3-b6d7-e590895fe30a" />

- Validation in Azure, during the review and creation of a virtual machine, involves Azure verifying your configuration settings to ensure they comply with requirements such as valid licensing, resource availability, and correct network settings. This step ensures that everything is properly configured before deployment, thereby preventing errors.
<img width="338" height="61" alt="12_create-vm-2" src="https://github.com/user-attachments/assets/d141b517-e834-4227-97af-f224d78c8cb2" />

- Once the validation process is completed, click “Create” to finalize the creation of the virtual machine.
<img width="553" height="460" alt="Screenshot 2026-09-02 at 10 28 20 PM" src="https://github.com/user-attachments/assets/e8b88a7f-e6df-4691-b7f9-0fe5553f0c94" />

- Now your Azure VM should be deploying....–
<h2> Now your Azure VM should be deployed </h2>

<img width="2554" height="1243" alt="Screenshot 2026-09-02 at 11 00 49 PM" src="https://github.com/user-attachments/assets/bf25a326-0f15-44d2-8396-ca80fe8313bc" />

<h2> Use Remote Desktop to test Windows VM </h2>
 <img width="2554" height="1243" alt="Screenshot 2026-09-03 at 5 28 46 PM" src="https://github.com/user-attachments/assets/1a13e090-4adc-4720-8574-399369ec04ad" /> 

 - 💻 RDP from a Mac to a Windows VM
Download Microsoft Windows App from the Mac App Store.
Open the app and select Add PC.
Enter the VM's Public IP Address.
Enter your Windows VM username and password.
Click Connect to access the VM remotely.

- 🪟 RDP from Windows to a Windows VM
Press Windows Key + R.
Type mstsc and press Enter.
Enter the VM's Public IP Address.
Click Connect.
Enter your Windows VM username and password.
You are now connected to the VM through RDP.

- RDP (Remote Desktop Protocol) lets you control a Windows virtual machine from another computer as if you were sitting directly in front of it.

<img width="2554" height="1243" alt="Screenshot 2026-09-03 at 5 30 51 PM" src="https://github.com/user-attachments/assets/c5bac19c-178f-445d-814e-3600b8fcb754" />

<h2> Conclusion </h2>

- This project showcases the immense power and versatility of Microsoft Azure in creating a virtual machine. It provides hands-on experience with both Windows and Linux environments in a cloud setting. By leveraging Azure’s Resource Groups and virtual networks, users acquire crucial skills in configuring and connecting VMs. This practical experience deepens their understanding of virtualization and network management, laying a solid foundation for mastering virtual machine deployment and virtual network setups in cloud environments.

   
   
