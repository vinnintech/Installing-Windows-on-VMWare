<p align="center">
<img src="https://imgur.com/SesjIjk" height="80%" width="80%" alt="Windows 11"/>
<br/>
  
# Installing Windows on VMware
This guide shows you how to install Windows 11 from scratch on VMWare. It includes downloading the necessary .isos, software, and complete VMWare settings and installation. Ideally for testing, repairing, and development. <br/>
(Can be used on any hypervisor 2 software such as VirtualBox, Parallels, etc.)

## Download VMWare Workstation Pro
- When Installing VMWare Workstation, you have to go to [Broadcom.com](Broadcom.com), and create an account with them.
  ![Image](https://github.com/user-attachments/assets/b89e38bd-3e2a-4d4b-adb2-9a7d236aef7f)
- Once you have created the account head over to the menu settings on the left hand side, click My Downloads and where it says "Free Downloads available" click "HERE"
  ![Image](https://github.com/user-attachments/assets/284d96fc-7c68-4b47-ae51-b708aa91de41)
- In the search bar type "Workstation" and select VMWare Workstation Pro
- Choose your version, in this case we will use Pro 17. 0(For Windows)
- Select the most recent patch update (17.6.4)
- Select the download button and in the browser a download should have begun
- Once completed run the file <br/>

- You may be prompted with a pop-up, choose yes.
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/f7ffaa9f-9a70-4c63-94f4-23d2de418a94" /> <br/>
## Installing VMware Workstation Pro
1. Select Next on the setup wizard.
2. Accept Terms of services in the License Agreement
3. Choose your installation destination. <img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/acb011bc-f3de-49aa-a6ea-4e2e7c223ebd" /> <br/>
4. Confirm User Experience Settings
5. Choose shortcuts
6. Once complete select "Install"
7. We have successfully installed VMware Workstation Pro
8. <img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/0d135c29-677b-43ba-a51a-74615b21beac" />
## Download Windows 11 ISO
1. [Go to Windows Download Site](https://www.microsoft.com/en-us/software-download/windows11)
2. Scroll till you see the ISO
3. Confirm and Download it
![Image](https://github.com/user-attachments/assets/ab485c97-1899-4558-b8dd-0c14e19fd3d5)

## Create a new Virtual Machine
1. Open VMware previously installed and you will see a fresh page where you will create your virual machine.
2. Select Create a New virtual Machine
3. Choose Custom(advanced) installation.
   
   (For this lab we will be configuring our machine ourselves, though you can skip this and choose "Typical(recommended)."
   <img width="584" height="587" alt="Image" src="https://github.com/user-attachments/assets/961df73e-5628-4a29-8278-3a14fbf7cc70" />
4. Select next, then this is where we will use the iso file we downloaded from Microsoft.
   <img width="545" height="555" alt="Image" src="https://github.com/user-attachments/assets/edd343db-62a2-4017-bd3d-d50a94089b66" />
5. Name your virtual machine and choose location
6. Here we will note down the Encryption information. <br/>
(**DO NOT LOSE THIS, YOU ARE NOW THE ADMIN OF THIS WORKSTATION**)
<img width="564" height="574" alt="image" src="https://github.com/user-attachments/assets/32dc0d55-4cbc-45ef-b792-b95740d84e02" />

7. Select Firmware type
    - `UEFI > Secure Boot`
8. Configure your processors
    - Number of processors: 1
    - Number of cores per processor: 4
    <img width="593" height="600" alt="image" src="https://github.com/user-attachments/assets/ad5384af-dcfc-4b38-b4c2-838e8d4ef853" />

9. Allocate memory for your vm, we will be using 16GB of RAM for ours (16384 MB)
<img width="631" height="636" alt="image" src="https://github.com/user-attachments/assets/d42e26f5-a281-418b-8197-83d0e85f8002" />

10. Choose NAT network connection
11. Proceed with recommended I/O controllers
12. Recommended Disk Type
13. Create a new virtual disk
    <img width="622" height="629" alt="image" src="https://github.com/user-attachments/assets/dadd4b4c-6db9-42af-af7c-968db5c1314c" />
    
14. Give your VM disk capacity.
    - 64 GB's will work fine to run our applications
    - Don't allocate all disk space, split virtual disk into multiple files
<img width="570" height="571" alt="image" src="https://github.com/user-attachments/assets/f686e2f4-4328-407f-a180-3573b29f202d" />

15. Name your disk file.
    
16. Confirm everything and Finish to create our new Virtual Machine
<img width="368" height="367" alt="image" src="https://github.com/user-attachments/assets/83eb87db-93cf-49a1-be8f-1222c7ebfee0" />

