# Active-Directory

## Objective

Project meant to develop skills related to Active Directory services. Gain insight into how remote servers can use virtualization to host resources and have another machine access the Active Directory to be able to login. Useful to understand Identity and Access management in systems.

### Skills Learned

- Host VMs on Virtualization software (Oracle Virtual Box) including Domain Controller server and Client machine.
- Set up Active Directory Services on an ISO Server 2019.
- Work with DHCP and DNS to provide network access and supply client with IP address lease and scope.
- Powershell script to create 1000+ users with relevant OU information.
- Create a client machine with access to the internal network and the web via Domain Controller.

### Tools Used

- Virtualization
    - Oracle Virtual Box
    - Windows 10 ISO
    - Server 2019 ISO
- Active Directory Services
- DHCP, DNS, RAS/NAT

## Steps

<p align="center">
  <img src="https://i.imgur.com/dYYhdVx.png" height="50%" width="50%" alt=""/> <br/>
  High-level overview diagram <br/> <br/>
</p>

- Set up Server 2019 on Virtual Box (Domain Controller)
    - After installation of the server, change network settings to have an internal network and NAT.
    - Set IP address for Internal network
        - Assign IP address for Internal & DNS.
- Install Active Directory Domain Services
    -	Post-deployment configuration (Create domain and admin account for AD DS).
-	Install RAS/NAT – So that client can use private DC network and access the internet
-	Set up DHCP on the server for clients to get IP address to access the internet
-	Execute PowerShell script to create new users on AD
-	Create a Windows client and log in using the relevant credentials
    -	Test for connectivity to DC and access to internet (using Echo Request Ping).

## Workbooks

<p align="center">
    <img src="https://i.imgur.com/vExTRxa.png" height="50%" width="50%" alt=""/> <br/>
    Final showcase of DC (running AD and DHCP) and Client machine (successfully connected to DC) <br/> <br/>
    <img src="https://i.imgur.com/OMNH3Gw.png" height="50%" width="50%" alt=""/> <br/>
    Settings of Domain Controller on Server 2019 <br/> <br/>
    <img src="https://i.imgur.com/OPmwxi5.png" height="50%" width="50%" alt=""/> <br/>
    Virtual Machines used for hosting DC and Client1 used in this project <br/> <br/>
</p>

 
## References

Josh Madakor. (2021, January 4). How to Setup a Basic Home Lab Running Active Directory (Oracle VirtualBox) | Add Users w/PowerShell [Video]. YouTube. https://www.youtube.com/watch?v=MHsI8hJmggI
