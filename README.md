# Installing Active Directory on Windows Server 2022 in a VMware Virtual Machine
This guide offers step-by-step instructions to set up **Active Directory (AD)** on **Windows Server 2022** running in a **VMware Virtual Machine (VM)**. Active Directory is a vital service for managing network resources, users, and security policies in a domain environment. 

By following this guide, you'll set up a virtualized domain controller, along with creating groups and users for your domain

## Requirements

- VMware Workstation or Player
- Windows server 2022 ISO file
- At least 2GB of RAM, 60GB of disk space, and 2 processors allocated to your virtual machine for optimal performance

## Installation Steps

### Step 1:Download Windows Server 2022 ISO File

Search for **"Microsoft Windows Server 2022 free download"** on Google and click on the link for **Windows Server 2022 | Microsoft Evaluation Center**.

![Image](https://github.com/user-attachments/assets/2d80996d-714c-46c6-8aa6-70868b13363c)

The following screen will appear. From there, select your preferred language and choose the **ISO download** for the **64-bit edition**.

![Image](https://github.com/user-attachments/assets/cc3810e8-2a7f-4ff4-a159-5e28dca53d84)

After clicking the link, the Windows Server ISO file will begin downloading. Allow the download to complete, and once it's finished, navigate to your **Downloads folder** to verify that the file has been correctly downloaded

![Image](https://github.com/user-attachments/assets/b2a6a258-0c89-4c4a-b2ed-205b96433e5a)


### Step 2: Creating a New Virtual Machine for Windows Server 2022

**Launch VMware Workstation** and select the option to **Create a New Virtual Machine**.

![Image](https://github.com/user-attachments/assets/dd69f1c5-f758-4cac-9dc0-d8f5a7f0bd45)

The next screen will prompt you to choose a configuration. For personal and learning purposes, leave the default option (**Typical**) selected, and click **Next**.

![Image](https://github.com/user-attachments/assets/5ad51b0d-c444-45ab-986f-03a36e31dda6)

You can browse and select the operating system here, or choose to do it later. For now, select the second option to **Install the operating system later**, then click **Next**.

![Image](https://github.com/user-attachments/assets/57c00151-c8ff-4ff4-b676-06e0ac1af980)

![Image](https://github.com/user-attachments/assets/7bb4c263-07e3-435a-8330-3d1d2bddf676)

Now, select the guest operating system and its version. Choose **Windows** as the OS, and set the version to **Windows Server 2022**, then click **Next**

![Image](https://github.com/user-attachments/assets/3f0be559-11b3-4ee8-b133-d37232a30355)

![Image](https://github.com/user-attachments/assets/ddaa577a-0cf5-4608-8de0-952ecf586105)

You can either change the virtual machine name or leave it as the default

![Image](https://github.com/user-attachments/assets/fd17cdff-6904-4db7-8eb2-dbf69c00bc32)

The screenshot below shows that you can customize the disk capacity, but the recommended disk size for Windows Server 2022 is 60GB. It’s best to leave it set to the default and click **Next**

![Image](https://github.com/user-attachments/assets/5483e5ec-e2cc-42db-b7c3-9c54fb2f117d)

After configuring all the settings for the virtual machine, click Finish to complete the setup.

![Image](https://github.com/user-attachments/assets/c1131c91-d02b-477c-a589-e7e5ef7fcae6)

### Step 3: Setting up Active Directory in windows server 2022

The screenshot below shows the Windows Server 2022 in virtual machine

![Image](https://github.com/user-attachments/assets/939b2d25-3454-4f80-b948-46f4545486b9)


On the left side My computer-> windows server 2022-> Right click-> Settings

You can modify all VM settings, such as the processor, memory, and more

![Image](https://github.com/user-attachments/assets/cd859510-e3f3-49c1-bace-34fc850ad49d)

In the settings Select CD/DVD (SATA)

![Image](https://github.com/user-attachments/assets/ad71ef6b-642c-4565-a911-3f8ebffb4445)

As mentioned earlier, browse for the OS here. Select Use ISO image file, then browse to the downloaded file and click OK.

![Image](https://github.com/user-attachments/assets/27fb63ef-e532-484a-952c-d59e701eea0c)

Once all settings are configured, power on the virtual machine

![Image](https://github.com/user-attachments/assets/68c91cf2-96e3-4717-9bea-cb3c323ffd7d)

The language selection window will appear. You can leave it as the default or change the language if needed

![Image](https://github.com/user-attachments/assets/7c341050-94b3-4a8d-a096-269603d01361)

When the screen below appears, press any key on the keyboard to proceed to the Windows Install screen

![Image](https://github.com/user-attachments/assets/1495d892-05e1-4621-a1ab-e40034375a46)

If you don't press a key, the following error will appear

![Image](https://github.com/user-attachments/assets/7952e9b3-4aa8-4409-b36d-e6beb09802e2)

Click install to download OS

![Image](https://github.com/user-attachments/assets/49acf621-12d5-4b66-ad04-2cc9b8974b3c)

On the next screen, you'll see four operating system options. Make sure to select the one labeled "Standard with Desktop Experience" — without the Desktop Experience, you'll only get a command-line interface, not a graphical user interface (GUI)

![Image](https://github.com/user-attachments/assets/3e741a89-b242-4d87-91da-07ed344878ac)

![Image](https://github.com/user-attachments/assets/cd471d00-04f8-4a41-8ec9-7afa72d51136)

Accept the license agreement to proceed with the installation

![Image](https://github.com/user-attachments/assets/0ce361cf-8bf4-4714-80a8-fd766d27e7e2)

We need to select "Custom" on this screen because we're installing the OS on a new virtual machine. The "Upgrade" option is used only when an operating system is already installed and we want to update or upgrade it

![Image](https://github.com/user-attachments/assets/09480c54-d960-46d0-b3e0-510759e94f7a)

The screen below displays the disk partition that we configured earlier and click Next

![Image](https://github.com/user-attachments/assets/83900dbc-f1bc-4835-a53c-8dd3d66cb04a)

The OS installation has now started

![Image](https://github.com/user-attachments/assets/acecd27e-0d05-4e08-9bdc-544508e2cfde)

After the OS installation is complete, the screen below will appear, asking you to set a password for the Administrator account. Fill the password and Click Finish
 
![Image](https://github.com/user-attachments/assets/1c090f03-f4dd-4517-8f51-4ce2b4bfd327)

![Image](https://github.com/user-attachments/assets/f2b9dd70-dc71-40b3-ac75-7fa3e32c5104)

The home page will open. To unlock it, press Ctrl+Alt+Delete

![Image](https://github.com/user-attachments/assets/ec907f9d-6ec1-48bf-9b4b-61084142b776)

Now, enter the Administrator password to log in

![Image](https://github.com/user-attachments/assets/ab6c85eb-b45e-4d64-b569-70c655291189)

Once you log in, the Server Manager screen will open automatically

![Image](https://github.com/user-attachments/assets/8a93f535-8e4f-4a94-9dc2-a2a8dcaeaa6c)

Optional: If you want to check the version of the Windows Server, type winver in the Run dialog and click OK.

![Image](https://github.com/user-attachments/assets/3e3737fe-f3e2-4353-a6fc-b4579a1690d6)

![Image](https://github.com/user-attachments/assets/e248db7c-1e34-416e-b508-d0e9cc993e29)

Now, we’re going to install Active Directory. To start, go to Server Manager, which is the page that appeared when you logged in.

In the top right corner, click Manage and then select Add Roles and Features. The screen below will open click Next

![Image](https://github.com/user-attachments/assets/058b482f-126a-4ecf-b206-849f7cf11e52)

In the next screen, select Role-based or feature-based installation and click Next.

![Image](https://github.com/user-attachments/assets/651fc491-90c6-486a-bc4d-1c854254fca0)

In the Server Selection screen, leave everything set to default and click Next

![Image](https://github.com/user-attachments/assets/d16ba9e9-bf03-4450-adc7-254e6e2b545a)

The primary goal here is to create a domain, and then add groups and users within that domain. So, select Active Directory Domain Services. When you click it, you'll see an option to Add Features — click that to proceed

![Image](https://github.com/user-attachments/assets/c967c71f-fa03-49db-b81b-938adfc1c5d2)

![Image](https://github.com/user-attachments/assets/fa5df5c8-ba6b-4962-9bf7-892721cfb327)

Optionally, you can also select additional features like DNS Server, DHCP, Remote Access, etc., depending on your requirements

![Image](https://github.com/user-attachments/assets/b9e4c7b7-aace-462a-a11e-092fe7d625f0)

Since we selected Active Directory Domain Services in the previous screen, Group Policy Management will be automatically checked in the next screen. Make sure it remains checked before proceeding amd click Next

![Image](https://github.com/user-attachments/assets/0610e1f0-6f53-4c94-9f80-5ef0c0864a5b)

TThe AD DS and Remote Access options are provided for your knowledge. Review the information and click Next to proceed. t

![Image](https://github.com/user-attachments/assets/92b03302-287c-4dcc-b5a1-bc0b2b140ae9)

![Image](https://github.com/user-attachments/assets/b2064e8f-266a-4361-8ab6-9d0ae47e645e)

In the following screens, check all three options and click Next. As a beginner, you don’t need to worry too much about these settings right now and click next

![Image](https://github.com/user-attachments/assets/fd194a46-0621-461b-bc42-cb061df7c632)

![Image](https://github.com/user-attachments/assets/99a24186-7614-4787-ab4a-9d7edb7835d1)

"Click Next until you reach the confirmation screen, where you can review all your selected options. Once confirmed, click Install to proceed

![Image](https://github.com/user-attachments/assets/6dcd66f9-708b-4f08-bfd3-c89cbd03970e)

![Image](https://github.com/user-attachments/assets/3484c874-f4db-4e30-9cfa-019d143cc47e)

![Image](https://github.com/user-attachments/assets/c7a1d6d2-5745-4e18-b65c-daef04ee11e5)

![Image](https://github.com/user-attachments/assets/9bbe5b74-4a46-4a80-9c63-dc8cd2554fe2)

![Image](https://github.com/user-attachments/assets/3f7c1fd1-38e4-4045-85ab-0b309fc9e22a)

Once the installation is complete, click Promote this server to a domain controller on the same page to begin the domain configuration

![Image](https://github.com/user-attachments/assets/38a25304-3486-4583-9587-45ea492bf83a)

In the next screen, you'll see the Deployment Configuration. Since we’re creating a new domain, select Add a new forest
![Image](https://github.com/user-attachments/assets/8547fb88-d60a-44d4-a66d-fdc46f7ed03b)

When selecting the root domain, make sure the domain name ends with .local (e.g., IT.local). This is because the domain is intended for local use only. Failing to do so may result in the error below

![Image](https://github.com/user-attachments/assets/928465ae-3ae0-446f-8701-22df47b5942b)

The following screen will display the new forest with the domain name you entered (e.g., IT.local). Click Next to continue.

![Image](https://github.com/user-attachments/assets/f704b736-aa67-44c9-af47-f3beadba8069)

In the Domain Controller Options section, the Forest Functional Level is set to Windows Server 2016, as it is the most recent version available. Now, you can create a password for your domain

![Image](https://github.com/user-attachments/assets/aaf09f29-53b7-4fc4-891a-1034ac8144d5)

Click Next for the DNS Options.

In the Additional Options, make sure the NetBIOS name matches the root domain name (e.g., IT if your domain is IT.local).

![Image](https://github.com/user-attachments/assets/b273c6ec-465a-4305-be2f-d71146d978fe)

After that, click Next for the Paths and review the options. Once everything looks good, proceed to the Prerequisites Check. Once the system verifies everything is correct, click Install to begin the domain promotion process.

![Image](https://github.com/user-attachments/assets/7aa926e4-b3b5-4431-b94b-f5a9af15ee9f)

Once the installation is done, restart the system. When it boots up, the Windows login screen will display your domain name

![Image](https://github.com/user-attachments/assets/55841ed1-4a9a-4095-9abb-de43193fe44f)

![Image](https://github.com/user-attachments/assets/6a85ef99-9922-4062-a755-4143a8465b88)

When you click Start and navigate to Windows Administrative Tools, you'll be able to see the tools you installed, such as Active Directory Users and Computers, Group Policy Management, and others

![Image](https://github.com/user-attachments/assets/a14975ec-0749-4dba-8121-a629c0038056)


### Step 4: Setting up Organizational Units(OU), Groups and Users in Active directory







