# Installing Active Directory on Windows Server 2022 in a VMware Virtual Machine
This guide provides detailed instructions for setting up **Active Directory (AD)** on **Windows Server 2022** within a **VMware Virtual Machine (VM)**. Active Directory is a vital service for managing network resources, users, and security policies in a domain environment. 

By following this guide, you'll create a virtualized domain controller, perfect for testing, learning, or development purposes.


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

Once you click the link, the **Windows Server ISO file** will begin downloading. Allow some time for the download to finish. When it's 100% complete, navigate to your **Downloads** folder and verify that the file is correct and fully downloaded.

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

The screenshot below shows that you can customize the disk capacity, but the recommended disk size for Windows Server 2022 is 60GB. It’s best to leave it set to the default and click next

![Image](https://github.com/user-attachments/assets/5483e5ec-e2cc-42db-b7c3-9c54fb2f117d)

Once all the settings are configured for the virtual machine, click Finish to complete the setup

![Image](https://github.com/user-attachments/assets/c1131c91-d02b-477c-a589-e7e5ef7fcae6)

### Step 3: Setting up Active Directory in windows server 2022

The screenshot below shows the Windows Server 2022 in virtual machine

![Image](https://github.com/user-attachments/assets/939b2d25-3454-4f80-b948-46f4545486b9)


On the left side My computer-> windows server 2022-> Right click-> Settings

You can modify all VM settings, such as the processor, memory, and more

![Image](https://github.com/user-attachments/assets/cd859510-e3f3-49c1-bace-34fc850ad49d)

In the settings Select CD/DVD(SATA)

![Image](https://github.com/user-attachments/assets/ad71ef6b-642c-4565-a911-3f8ebffb4445)

As mentioned earlier, we will browse for the OS here. Select Use ISO image file and then browse to select the file and click ok.

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













