# Active-Directory-Lab
## Downloaded VMware Workstation Player, Windows Server 2019 ISO, and Windows 10 ISO.<br>
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/8f24ebc7-26a1-4ba4-970a-1f7a9770e040)
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/6c3369ce-23d9-4570-88dc-b80c013292e5)
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/144bdbc8-11de-4fbd-8ace-5ac663a12243)
For all 3 downloads I navigated to google chrome and searched VMware and Microsoft eval center website for VMware workstation Player, Windows Server 2019 ISO and Windows 10 Enterprise ISO. I downloaded the files and then ran the VMware installation. This will allow me to start installing the virtual machines with VMware and begin my Active Directory Lab environments.

## Created virtual machines for Windows Server 2019 and Windows 10 Enterprise.
- To create a virtual machine I opened VMware and clicked on Create a New Virtual Machine. .<br>
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/acf34b63-8702-4662-9dec-2ebf1780fea5)
- Selected I will install operating system later where I will put ISO file in after some steps.<br>
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/f7a718cb-9e15-4999-962a-6e649c49753c)
- Selected the correct Guest Operating System for the virtual machine I am creating.<br>
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/0ef81030-0658-40b5-9ec1-93fed09d79be)
- Created a name for my virtual machine and I selected a location on my drive for the files.<br>
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/db6fe610-474a-4fbb-9938-84fed13cc65f)
- I selected 60 GB storage size because thats all I need for this lab and selected Split virtual disk into multiple files if I ever want to move my VM to another computer.<br>
![5](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/609aca66-0d68-4a89-b975-11db0063a03f)
- I decided to not change the hardware because it was enough for this lab.<br>
![6](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/a87d8dc6-0340-4732-b2c5-4278e0a64ed1)
- Selected my virtual machine from the VMware main page and pressed edit virtual machine settings.<br>
![7](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/4e59aa9e-360b-4ece-8eed-74cd64e74fb0)
- Selected CD/DVD (SATA) and switched it to Use ISO image file and browsed my ISO file for Windows Server 2019. Then went back to my virtual machine and powered it on.<br>
![8](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/3c449eef-fd67-4974-b81e-fbe7336b05f5)
- Selected english and pressed install to begin the Windows setup process.<br>
![9](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/ef98582e-4917-49de-9159-279909433e0e)
- Selected Windows Server 2019 Standard Evaluation to have a GUI and accepted license terms message.<br>
![10](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/b9af7e4e-657f-4f23-8d93-23e29a72b3b9)
- Selected Custom Install advanced and pressed next because I dont need to add more drives for this lab.<br>
![11](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/4dd02055-dd45-4634-9956-7bc6d6a20400)<br>
![11](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/e7efdec8-43d8-48c9-b5f6-b86a1e3367cc)
I created the Windows Server 2019 virtual machine using VMware's Virtual Machine wizard. I also created two more virtual machines using the same steps except I changed the names and used Windows 10 Enterprise edition to add them for this lab.

## Renaming Computers.
- Opened file explorer and right clicked this pc and clicked properties to see the system information.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/f9aebd5f-0d3e-44ae-90f8-37a412c0e3ed)
- Opened change settings next to Computer name to open System Properties.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/ef214e8f-3317-4826-b7a6-02b6bcfa5940)
- Clicked change next to rename computer explanation to open Computer Name/Domain Changes.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/103dc7d2-a0e8-4e30-bdc7-0a4e1baee15d)
- Typed in a different computer name and left this computer on Workgroup for now. Pressed ok and restarted computer.
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/29b6f91b-64e1-4c02-90e4-9af92a033fa2)
I renamed the Windows server 2019 computer and the Windows 10 Enterprise computers as well with the same steps as above.

## Adding Active Directory with Add Roles and Features Wizard in Server Manager.
- Opened Server Manager and pressed Manage and than pressed Add Roles and Features to open the Add Roles and Features Wizard.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/3bc28b3b-f7d3-4771-8822-8c4257a57c81)
- Verified my Admin password strength, network settings, security updates and pressed next.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/c1000136-fc90-4c81-863c-b5a34d9fc9b3)
- Selected Role-based or feature based installation for single server and pressed next.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/f665df43-7dba-4804-8829-f18b18ecf12b)
- Selected my server from the server pool and pressed next.
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/79bb7d09-80d2-4fe0-873b-59c270a096cd)
- Checked Active Directory Domain Services from server roles and click next.
![5](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/f0ff77c7-ee2b-40dc-8063-52e84bb29efb)
- Used default features that are already checked and pressed next.
![6](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/ff94af42-bb72-4e95-9f51-0ce04e90dffa)
- AD DS page stating information about Active Directory Domain Services I read and pressed Next.
![7](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/67578c12-8dd9-4126-b9a9-df92fbe165ba)
- Confirmed and pressed install to start the installation process.
![8](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/c8cbff3d-28ef-4ee8-a3d8-1532d993fca2)
- After installation is successful pressed promote this server to a domain controller.
![9](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/ade07793-9012-4648-833a-45a6e111e040)
- Check add a new forest becuase I dont have an existing domain yet or an existing forest. Typed in my Root domain name and pressed next.
![10](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/ea6c6461-d538-4fd0-8c97-afec8421f6c5)
- Used default options and created a DSRM password and pressed next.
![11](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/411577e5-d468-48ff-bcb0-93214e4ff4d0)
- Pressed next on DNS options because I dont need to create a DNS delegation yet for this lab.
![12](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/950c0967-f4e8-4aba-9ea4-b8049151d9c3)
- Pressed next on additional options.
![13](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/e6ed65bd-c68a-46b4-a1e9-12e03b19546a)
- I left paths as default because the file paths are fine in the C: drive for this lab and clicked next.
![14](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/a43ba0af-b530-43e9-b243-c71aad338bb0)
- Reviewed my selected options and pressed next when I finished.
![15](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/670b498d-9e8a-4fc1-9a15-ee88cf800a1e)
- Pressed install on prerequisites check.
![16](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/ebc95ac7-3f57-4861-bb67-4630d0f4b00c)
- Pressed Tools on Server Manager and opened Active Directory Users and Computers to see if it installed properly.
![17](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/e95a50ea-6df7-406c-8818-a97e022ff8a8)
- I can see that the installation was a success.
![18](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/42f83dad-7588-4751-9d9c-5a052eb6c086)

## Assigning static IP Addresses to virtual machines.
- Opened start menu and pressed Control Panel to adjust settings.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/508184ec-a1b8-431d-95d6-b2acd68983e9)
- Pressed View network status and tasks under Network and Internet to open Network and Sharing Center.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/ccd5d3db-e4c3-4b99-afa3-40d955e37a2e)
- Pressed Change adapter settings to see Network Connections.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/ea432fa0-11bd-476f-9609-fb01a6fbffc6)
- Opened Ethernet0 Network and pressed properties to see items the connection is using.
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/f4e59024-e227-4a90-bd49-d2f092185213)
- Selected Internet Protocol Version 4 TCP/IPv4 and pressed properties.
![5](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/b66c70d8-5b11-4fb2-bfc0-350c8def471a)
- Selected the Use the following IP address option and Use the following DNS server addresses and input static IP address.
![6](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/2d00432d-0f32-4ba6-a9c5-660f5b8bcb0e)
- Opened Virtual Machine Settings to select Network Adapter settings from NAT to Host-Only so there is no issues connecting to the domain.
![7](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/b706a081-613a-4244-8e3a-6acba45a9d1f)

## Adding virtual machines to the domain.
- Opened File Explorer right clicked This PC and pressed properties to open System.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/a95e4a00-967c-4ed1-8044-1cdbb2727e3d)
- Scrolled down and pressed Rename this PC (advanced) to open System Properties Computer Name tab.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/77905240-89cb-4d61-a45c-a6d0a1973969)
- Pressed change to open Computer Name/Domain Changes.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/3c57f2ea-976a-47f4-a3a2-6dc6bfde4527)
- Select Domain, type in domain name and press ok to connect to domain.
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/bf68a668-7cfe-4451-bde7-9e9518033d28)
- I got a welcome message for connecting to domain.
![5](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/9247e707-5430-4e6c-9b33-bdeaa0e9002f)
- Opened Active Directory Users and Computers and under the Computers branch I can see the computer added to the domain.

## Enabling Administrator account.
- Opened File Explorer and right clicked This PC and pressed Manage to open Computer Management.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/70320530-31a9-4a2a-9fae-51920c885af4)
- Under Local Users and Groups selected Users to see list of users.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/8a0a0192-9551-40a6-a9d2-75236c839851)
- Opened Administrator user and unchecked Account is disabled to be able to log in as Administrator.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/26304f0d-e047-4d30-a8f6-ea06290a872f)

## Installing RSAT Tools to Helpdesk computer.
Typed programs into search bar and opened Add or remove programs to open Apps and features.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/53945054-7fef-4b81-864b-802bb67c9370)
Pressed Optional features.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/bbd93cdc-3544-4e15-b919-f9ae543cc242)
Pressed Add a feature and searched for RSAT and selected the specific ones I need and started installation.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/5cea933a-5617-415f-8a51-6c82f81c67cb)

## Creating Users in Active Directory Users and Computers.
- Opened Active Directory Users and Computers from Server Manager Tools selection.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/3453f44a-2fd3-423d-9407-4e6bfd446c63)
- Under coretlab.com and Users I right clicked open space and selected New and User from drop down.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/83b500f9-45b6-456e-b456-0434cf3f4d19)
- Typed in name and logon info and pressed next.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/fe8217c6-3245-4dbe-9bc3-29db2ec1d045)
- Created a password and checked user must change password at next logon and pressed next.
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/acc0770b-edaf-4024-8e3c-d561ed2f0a9e)
Reviewed the selections I made and pressed finish.
![5](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/df17aac6-58f8-4a29-ba61-0df190ddb36e)
Confirmed the user has been created in users by seeing there name.
![6](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/bb6e0664-6fec-46c2-ad12-c822383b9d11)

## Copying User in Active Directory Users and Computers.
- Opened Active Directory Users and Computers from shortcut pinned to taskbar. Selected a user to copy and right clicked and slected copy.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/9b75d112-42d1-4d80-8868-519e804bfe8d)
Typed in a new name, logon, and pressed next.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/fc03a22a-388e-406d-95d0-3c5196359257)
Set a password and pressed next.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/9e1c07e9-06c4-432f-8f61-1a8aee5c39a2)
Reviewed my selections and pressed finish to create user.
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/b347eca9-a189-4c1a-9088-f5669bba9d2f)

## Creating an organizational Unit in Active Directory Users and Computers.
- Opened Active Directory Users and Computers. Right clicked my forest and selected new and pressed Organizational Unit.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/a2c8b5c5-e92f-40d4-ad67-bf5ea6e03aa2)
- Named the Organizational Unit and pressed ok.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/da1d944b-bddb-4400-a428-7fc27887dec2)
Confirmed the Organizational Unit has been created by seeing it under coreylab forest.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/9e5ca857-3bcb-4909-8004-006bb29b3f50)

## Creating a Security Group in Active Directory Users and Computers.
- Opened Active Directory Users and Computers. Right clicked on users, selected new and pressed Group.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/35ccd331-483b-4a17-83c1-9d04ad19c5f9)
- Named group and selected Security and pressed Ok.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/214ae764-dfc0-4486-859a-b60d8364042f)
- Opened the security group properties.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/9cc3f145-cc60-42f3-a7c8-15071e83d24d)
- Switch to Members tab and press add to select a user.
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/af59f95b-5303-4afe-99fd-21652c5a512c)
- Added Helpdesk1 User to the Security Group pressed apply and OK.
![5](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/a76eb9dc-60e4-409e-a5cb-c74be6c9b393)
- Double checked User properties to see if it was in the member of section.
![6](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/fbf4d2ab-1932-4db8-a689-35bdbb4676ac)

## Unlocking Account that has been locked out in Active Directory Users and computers.
- I opened Active Directory Users and Computers and right clicked the user and pressed Enable Account.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/adad797e-701e-4441-ab00-29ae32f76255)
- Another way I unlocked account is in Active Directory Users and Computers and opening users properties.
![2 2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/eebc5615-be6f-4c77-8dcb-f394c2781e29)
- Pressing Account tab in properties and checking Unlock account and pressing ok to unlock account.
![4 2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/2b31af1b-8043-4f4a-8d5b-7b5a8eeacb67)

## Resetting user password in Active Directory Users and Computers.
- Opened File Explorer right clicked the user and selected Reset Password.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/b3033ba3-3b26-4e64-92e3-6caeeaa54fe0)
- Typed the new password. Selected user must change at next logon and pressed ok to reset password.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/1d205d16-0d47-466a-b13e-b3c3f6c93e38)
- User typed in new temporary password.
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/9d589a0a-5ca4-42cc-9b34-aee9796d506e)
- Pressed ok to password must be changed message.
![5](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/2605308b-7ccc-4b28-8f58-6d8beba6006c)
- Typed in old and new password to update password.
![6](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/f48cc577-bcc8-4c1f-a049-5f0011a34f1b)
- Password successfully changed.
![7](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/12b30f97-c572-442d-84bd-626e7ca6c077)

## Unlocking user account that has been expired in Active Directory Users and Computers.
- User account has expired.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/c69b285c-276f-4c9a-9a1a-db05e17e6a86)
- Opened Active Directory Users and Computers and opened the users properties.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/f5f47a5e-5bd1-424d-ad9b-47a5380b899d)
- Opened the Account tab and account expired never option and selected apply and ok.
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/8a92c02a-4471-47f5-a99b-ee71efbfc878)
- Searched cmd in start search and opened Command Prompt.
![5](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/5e30db19-29e3-409e-9806-bffebfa9ca1e)
- Used net user command to double check if account expiration has been updated.
![6](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/c10e5c60-f9a3-46d6-9902-44cbf994727d)

## Reconnecting Computer that has fallen off the domain.
- Deleted the computer to simulate the computer falling off the domain.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/0d5019a9-8327-4bea-b713-41abbb51014c)
- Logged in to local Administrator account on the machine.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/c564548b-36d9-461f-baef-52ad36967036)
- I reconnected the computer to the domain.
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/4f34ff59-17e1-4f4d-a4ad-c45bc7aa6cfa)
- The computer is showing on the Computers section of my domain.
![6](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/add3345b-6f70-4ec8-8b99-e26056a88d6b)

## Creating share folder with Active Directory Server Manager.
- Opened Server Manager and pressed File and Storage Services.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/d6dbdb9e-b4d8-4c04-88bc-c14742f265be)
- Press Shares and in open space in shares right clicked and pressed New Share to open New Share Wizard.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/91fec839-9b9d-43c8-b0a0-5fd2ae61e865)
- Selected SMB Share - Quick because it suits this lab good.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/d7f6d853-3b58-445b-985c-a43d55f50847)
- Selected my server and the default path for this share folder. 
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/37eba796-8517-46c0-92c3-965322f78fd3)
- Typed in the Share name and pressed Next.
![5](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/85ec4e7e-791e-4fe7-9a3a-a19543632957)
- Left the Allow caching of share checked to have access offline and pressed Next.
![6](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/57c1ff73-3e0f-4555-9eac-d443647bf80e)
- Left permissions default to change later on in lab and pressed Next.
![7](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/10262497-37fb-42b8-b195-671430478e61)
- Confirmed the selections and pressed Create.
![8](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/a95b32bf-6738-4892-96cf-4ebb58e40670)

## Creating share folder with File Explorer.
- Opened This PC pressed Local Disk (C:) then pressed Shares folder I created. Opened new Brand folder properties.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/6dbe630b-0a58-4c17-9828-ab43cae3dca9)
- In properties clicked Sharing tab and pressed Share.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/7276ffa6-0bb3-4e78-a66f-3768ca9e2d95)
- In Network Access I added user I want to map this share folder to.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/a77f5e64-74cd-4d70-90e2-8f0422bc2a9a)

## Mapping a Network Drive.
- Opened File Explorer and pressed This PC and selected Map network drive...
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/9b478028-6182-4de2-94cb-054a1ea8de75)
- Selected the drive letter and typed in network folder location checked Reconnect at sign-in and pressed finish.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/cadc976f-0a40-415f-95f8-5b340d4f613d)
- File Explorer shows on This PC that my drive has been mapped.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/f3221b53-4c3b-4c89-8236-16d4a1793d6f)

## Mapping a Network Drive in Active Directory Users and Computers.
- Opened Active Directory Users and Computers from my pinned shortcut on taskbar and slected IT and opened user properties.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/28479b9e-0344-4e59-85ec-4398d10e832b)
- In profile selected Connect P: drive and typed location of share folder then pressed Apply and OK.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/266a9168-d1d1-4daa-a9aa-2c3007930245)
- Creating a mapped drive after user logs on next.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/5d15beea-ccb2-44ab-ab25-e66bc10172b6)

## Remoting into second virtual machine computer using Remote Desktop Connection.
- Searched for and opened Remote Desktop Connection on start menu.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/59968b17-3794-4aa5-a70b-6a896a1f17a8)
- Typed in the second computer I wanted to remote into and pressed Connect.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/77210000-8b6f-4389-89ec-745680bab9ac)
- Used my credentials to connect and pressed OK.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/347d631e-8bfd-44b6-8ab2-73f9b43af390)
- From users computer pressed OK allowing the connection.
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/9f605b2d-618b-454b-a9a0-4f4dbcb82221)
- Successfully remoted into the computer.
![5](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/37550fac-e42a-4fcd-90d7-5f6c57b2acfa)

## Changing Default Domain Policy settings in Group Policy Management.
- Opened Server Manager selected Tools and opened Group Policy Management.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/c0881cd2-7ea2-4fe1-861c-2a889f5e5b03)
- Opened Forest, Domains, coreylab and right clicked Default Domain Policy and pressed Edit.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/e9503a09-cf1b-40cc-af6e-1ec72d939149)
- In Computer Configuration, Policies, Windows Settings, Security Settings, Account Policies, Account Lockout Policy edited Account Lockout Duration.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/4f800573-11fb-4b9a-b6d4-c1e841ff5b66)
- Under Password Policy edited Maximum password age.
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/f1f0ca8d-e7fb-4572-ac8d-9ebf9afce9a4)
- Right clicked on Default Domain Policy and checked Enforced on.
![7](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/d151ccfe-c43e-476e-8978-626754d0443b)
