# ProtonVPN
<p align="center">

![mage](https://github.com/jrford32/ProtonVPN/assets/101678489/3b2fff55-72f2-4d9b-a457-f332a65fddad)

</p>

<h1>ProtonVPN - Installation</h1>
This tutorial outlines the installation of the ProtonVPN (Virtual Private Network).<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- ProtonVPN

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Installation Steps</h2>

<p>

![image](https://github.com/jrford32/ProtonVPN/assets/101678489/cf077a17-7e0f-412c-b9d7-82764a4075a4)

</p>
<p>
To begin, we are first going to create a resource group in Microsoft Azure. I named it something simple such as "RG-VPN". Review and create your resource group.
</p>
<br />

<p>

![image](https://github.com/jrford32/ProtonVPN/assets/101678489/e8ae1227-0cb4-42e6-b743-1f06f87712b2)

</p>
<p>
Once the resource group has been created, create the virtual machine next. The virtual machine (VM) should use the Windows 10 operating system and should be set in a different geographic location. I used Asia for this lab.
</p>
<br />

<p>

![image](https://github.com/jrford32/ProtonVPN/assets/101678489/8a952103-a777-4ea7-b03b-382212c29374)

</p>
<p>
Once your VM has been deployed, make note of the public IP address that was created with it. You can either write it down or use 'Notepad' in Windows. The public IP address for this VM is 40.81.20.240.
</p>
<br />

<p>

![image](https://github.com/jrford32/ProtonVPN/assets/101678489/5ebd2668-db41-404f-ae5e-9cd60c93fcfd)

</p>
<p>
Start the VM by copy and pasting the IP address into Windows 'Remote Desktop Connection'. Input the login credentials you created when you created the virtual machine.
</p>
<br />

<p>

![image](https://github.com/jrford32/ProtonVPN/assets/101678489/7cf43451-26ec-4f68-ad55-e3ad08eca6da)

</p>
<p>
Inside your VM, go to the ProtonVPN website and create an account. Once your account is created, download the Windows VPN client to the VM. Once the VPN is installed, login using the account credentials you created previously and you will now be on the dashboard.
</p>
<br />

<p>

![image](https://github.com/jrford32/ProtonVPN/assets/101678489/6aead215-f7e2-4baf-afb5-10f937cab361)

</p>
<p>
On the dashboard, the left hand side shows multiple different countries that you are able to connect to. Unfortunately, the free version of Proton does not allow you to freely sleect your country so in this case, we are going to select "Fastest" and see what country/region the client provides us. Once you try to connect to the VPN, the remote connection to the VPN may disconnect. This is fine because it will eventually reconnect. In this case, we were connected to a server in Japan, likely due to us creating the VM in East Asia.

![image](https://github.com/jrford32/ProtonVPN/assets/101678489/dadb9cf5-66e9-48e8-86f0-5712089fdc0f)
  
</p>
<br />

![image](https://github.com/jrford32/ProtonVPN/assets/101678489/88e13833-2d1e-4856-9b98-56df01823271)
![image](https://github.com/jrford32/ProtonVPN/assets/101678489/3edd62a2-e34d-4a54-af34-67d47ae07a0a)

As a final test to see what the actual VPN does to our browsing, I searched sites such as Google and Netflix and as you can see, the language and URLs are showing in Japanese. On the Netflix website, you can see the subscription cost shown as JPY 790, which is Japanese currency.

<h1>Summary</h1>
In this project, I successfully installed Proton VPN on a virtual machine running Windows 10. The installation process involved setting up a virtual machine, configuring the necessary dependencies, and ensuring that Proton VPN was correctly installed and operational. The benefit of using a VPN allows for enhanced privacy by being able to mask your IP address as well as encrypt your internet traffic and secure sensitive information.
