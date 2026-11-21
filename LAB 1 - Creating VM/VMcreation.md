# Creating a Windows Virtual Machine in Azure

- Step 1: Under Azure Services in the Azure Portal we can click on the Virtual Machines menu. It will open the VM page of the portal, click on create option. For now we will go with first option. We can also search for the Virtual Machine using portal's search bar.

![Virtual Machine Menu in Azure Portal](./Snaps/Screenshot%202026-11-21%20182758.png)

![Inside VM Page of Portal](./Snaps/Screenshot%202026-11-21%20183321.png)

!['Create a virtual machine hosted in Azure'](./Snaps/Screenshot%202026-11-21%20184426.png)

- Step 2: After this we will see our main interface containing vairous tabs to configure the VM. For now we will leave most of these default but will highlight few important ones.

![Create VM Page](./Snaps/Screenshot%202026-11-21%20185517.png)

- Step 3: We have to choose a Subscription and a resource group inside the subscription. We can choose from existing resource groups from the subscription or create a new one.
![Subscription and Resource group VM](./Snaps/Screenshot%202026-11-21%20185911.png)

- Step 4: In the instance details section, we name the VM and choose a region with the Availablity Options. In the availablity options we will have 3 options:
  - No infrastructure redudancy required
  - Availability Zones (We will choose this for this Lab)
  - Virtual Scale Set
  - Availability Set
![VM Availibility Options](./Snaps/Screenshot%202026-11-21%20191131.png)

- Step 5: Next we choose a security type which configues VM secure. There are 3 types along with some extra config option:
  - Standard
  - Trusted Launch Virtual Machine (We will choose this for this Lab)
  - Confidential Virtual Machine
![Security Type in VM](./Snaps/Screenshot%202026-11-21%20191331.png)
![Security Type in VM](./Snaps/Screenshot%202026-11-21%20191348.png)

- Step 6: After this we choose a OS image. Azure already gives options to choose from or we can use our own custom image. Here we also select VM architecture.
![VM Image and Architecture](./Snaps/Screenshot%202026-11-21%20192025.png)

- Step 7: Choose the VM size by referring to VM size table which can be opened by clicking 'See all sizes' and we can even further customize the core. We choose a simple D series for our mini lab.
![VM Size](./Snaps/Screenshot%202026-11-21%20192617.png)

- Step 8: Create a admin username and password for VM to login
![VM Admin Account](./Snaps/Screenshot%202026-11-21%20193033.png)

- Step 9: We need to setup a port for internet access to VM. As this is a test lab we will go with RDP (3389) which will enable us to acess the VM using RDP protocol. We have other ports as well like HTTPS (443), HTTP (80), SSH (22).
![Ports VM](./Snaps/Screenshot%202026-11-21%20193721.png)

- Step 10: We change our tab to Disks where configure our VM storage. For this lab we are going to leave as it is.
![Disks Size VM](./Snaps/Screenshot%202026-11-21%20193721.png)

- Step 11: We now change the tab to Networking. A VM must be part of a virtual network. We can get some virtual networks from the selected regions. We can even create a new VNet. We option to config subnet and public IP.
![VM Network](./Snaps/Screenshot%202026-11-21%20194958.png)

- Step 10: We will keep rest of the things as it is and do a review and create. It will take few mins to deploy. Some other resouces required to run the VM will also be created automatically.

![Review details VM creation](./Snaps/Screenshot%202026-11-21%20195527.png)
![VM creation](./Snaps/Screenshot%202026-11-21%20195553.png)
![VM Created](./Snaps/Screenshot%202026-11-21%20195850.png)
