# ActiveDirectory-HomeLab-1000Users
First active directory homelab project
# ActiveDirectory Homelab 1k Users

## Objective
This project served as an entry-level project for getting a better understanding of Windows Server 2019 and Active Directory. The lab was conducted in a VirtualBox environment. The environment contained a Windows Server 2019 virtual machine (VM) as the domain controller and a separate Windows 10 VM which served as a client machine to verify user account functionality. For networking, I configured Network Address Translation (NAT) and routing for internal and external network access, and enabled Dynamic Host Configuration Protocol (DHCP) for automatic IP assignment. To create a simulated AD environment, I used a PowerShell script that automated the creation of 1,000 user accounts. Through this lab I gained experience in Windows Server administration, AD management, networking, and automation using PowerShell. I also gained a better understanding of Active Directory and how domain controllers operate. 


### Skills Learned
- Windows Administration
- Active Directory management
- Virtualization
- Networking

### Tools Used
- VirtualBox
- Windows Administration Tools

## Steps
1. Download Windows 10 iso and servers 2019 iso
  a. These iso images will be on two separate VMs
2. Create first VM
  a. This will be our domain controller and house AD
  b. Have two network adapters
    i. One connects to the outside internet
    ii. Two connects to the virtualbox private network that the clients will connect to
3. Install server 2019 on VM
  a. Assign IP addressing for the internal network
  b. External network will automatically get IP addressing from your home network
  c. Name server
4. Install AD and create domain
5. Configure NAT and routing 
  a. Enables clients on the private network to connect to the internet through the domain controller
6. Setup DHCP on the domain controller
  a. Windows 10 machine will automatically get an IP address
7. Create 1k users in AD
  a. Run a PowerShell script on the domain controller for this
8. Create another VM
  a. Install Win10
  b. This will be connected to the private virtual box network
  c. Name machine client 1
  d. Join to the domain
9. Log into client 1 with one of the domain account

<a href="https://lucid.app/lucidspark/c160ad66-f0d4-4f8a-a670-056dfa1392a9/edit?viewport_loc=-4092%2C-1642%2C7115%2C3219%2C0_0&invitationId=inv_244ca1dd-0643-498d-891b-d352ef4b7589">Network Diagram</a>
