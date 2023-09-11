## Active-Directory-Lab
## Downloaded VMware workstation player, Windows Server 2019 ISO, and Windows 10 Enterprise ISO from their websites and installed VMware onto my computer.<br>
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/14165504-a721-4c69-801b-07803518fa0e)
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/1d2baae9-fe29-4a55-a204-9f4e56462eca) 
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/e104bf42-998e-4b72-919b-4bc9ba7f7c6c)
## Explanation: For all 3 downloads I navigated to google chrome and searched VMware and Microsoft eval center website for VMware workstation Player, Windows Server 2019 ISO and Windows 10 Enterprise ISO. I downloaded the files and then ran the VMware installation. This will allow me to start installing the virtual machines with VMware and begin my Active Directory Lab environments.

## Created virtual machine for Windows Server 2019 ISO
- ### To create a virtual machine I opened VMware and clicked on Create a New Virtual Machine. .<br>
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/acf34b63-8702-4662-9dec-2ebf1780fea5)
- ### Selected I will install operating system later where I will put ISO file in after some steps.<br>
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/f7a718cb-9e15-4999-962a-6e649c49753c)
- ### Selected the correct Guest Operating System for the virtual machine I am creating.<br>
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/0ef81030-0658-40b5-9ec1-93fed09d79be)
- ## Created a name for my virtual machine and I selected a location on my drive for the files.<br>
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/db6fe610-474a-4fbb-9938-84fed13cc65f)
- ## I selected 60 GB storage size because thats all I need for this lab and selected Split virtual disk into multiple files if I ever want to move my VM to another computer.<br>
![5](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/609aca66-0d68-4a89-b975-11db0063a03f)
- ## I decided to not change the hardware because it was enough for this lab.<br>
![6](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/a87d8dc6-0340-4732-b2c5-4278e0a64ed1)
- ## Selected my virtual machine from the VMware main page and pressed edit virtual machine settings.<br>
![7](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/4e59aa9e-360b-4ece-8eed-74cd64e74fb0)
- ## Selected CD/DVD (SATA) and switched it to Use ISO image file and browsed my ISO file for Windows Server 2019. Then went back to my virtual machine and powered it on.<br>
![8](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/3c449eef-fd67-4974-b81e-fbe7336b05f5)
- ## Selected english and pressed install to begin the Windows setup process.<br>
![9](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/ef98582e-4917-49de-9159-279909433e0e)
- ## Selected Windows Server 2019 Standard Evaluation to have a GUI and accepted license terms message.<br>
![10](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/b9af7e4e-657f-4f23-8d93-23e29a72b3b9)
- ## Selected Custom Install advanced and pressed next because I dont need to add more drives for this lab.<br>
![11](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/4dd02055-dd45-4634-9956-7bc6d6a20400)<br>
![11](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/e7efdec8-43d8-48c9-b5f6-b86a1e3367cc)
- ## Explanation: I created the Windows Server 2019 virtual machine using VMware's Virtual Machine wizard. I also created two more virtual machines using the same steps except I changed the names and used Windows 10 Enterprise edition to add them for this lab. Having virtual machines set up will allow me to begin installing Active Directory and continue my lab.

# Renamed Server Computer
- #### Opened file explorer and right clicked this pc and opened properties.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/f9aebd5f-0d3e-44ae-90f8-37a412c0e3ed)
- #### Open change settings next to Computer name.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/ef214e8f-3317-4826-b7a6-02b6bcfa5940)
- #### click change next to rename computer explanation.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/103dc7d2-a0e8-4e30-bdc7-0a4e1baee15d)
- #### typed in a different name and pressed ok and restarted computer.
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/29b6f91b-64e1-4c02-90e4-9af92a033fa2)
### Explanation: I renamed the server computer so it is easier to remember for me and more organized.

# Adding Active Directory with Add Roles and Features Wizard in Server Manager
- #### Open server manager and click manage and add roles and features.
![1](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/3bc28b3b-f7d3-4771-8822-8c4257a57c81)
- #### Verify Admin password strength, netgwork settings, and security updates and click next.
![2](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/c1000136-fc90-4c81-863c-b5a34d9fc9b3)
- #### Selected role based installation for single server and cick next.
![3](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/f665df43-7dba-4804-8829-f18b18ecf12b)
- #### Selected my server from the server pool and click next.
![4](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/79bb7d09-80d2-4fe0-873b-59c270a096cd)
- #### Check Active Directory Domain Services from server roles and click next.
![5](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/f0ff77c7-ee2b-40dc-8063-52e84bb29efb)
- #### Used default features that are already checked and clicked next.
![6](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/ff94af42-bb72-4e95-9f51-0ce04e90dffa)
- #### Page stating information about Active Directory Domain Services. Click next.
![7](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/67578c12-8dd9-4126-b9a9-df92fbe165ba)
- #### Confirm and click install to install roles and features.
![8](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/c8cbff3d-28ef-4ee8-a3d8-1532d993fca2)
- #### After installation click promote this server to a domain controller.
![9](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/ade07793-9012-4648-833a-45a6e111e040)
- #### Check add a new forest and type in root domain name and click next.
![10](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/ea6c6461-d538-4fd0-8c97-afec8421f6c5)
- #### Used default options and created a DSRM password on Domain controller options.
![11](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/411577e5-d468-48ff-bcb0-93214e4ff4d0)
- #### Click next on DNS options.
![12](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/950c0967-f4e8-4aba-9ea4-b8049151d9c3)
- #### Click next on additional options.
![13](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/e6ed65bd-c68a-46b4-a1e9-12e03b19546a)
- #### I left paths as default and clicked next.
![14](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/a43ba0af-b530-43e9-b243-c71aad338bb0)
- #### Review options and click next when done.
![15](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/670b498d-9e8a-4fc1-9a15-ee88cf800a1e)
- #### Press install on prerequisites check.
![16](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/ebc95ac7-3f57-4861-bb67-4630d0f4b00c)
- #### Press tools on server manager and open Active Directory Users and Computers.
![17](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/e95a50ea-6df7-406c-8818-a97e022ff8a8)
- #### We areable to open and see our domain forest.
![18](https://github.com/coreybruck/Active-Directory-Lab/assets/78772836/42f83dad-7588-4751-9d9c-5a052eb6c086)

## Creating an account









