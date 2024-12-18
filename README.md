"# Elias_VG2_Terminoppgave"

## 1. Plan
Im going to create a infrastrucute to a small company, that must have a domain, DNS, DHCP, and good file structure, And a step by step guide.

## 2. Required Softwares
- Hyper-V.
- ISO FILES
    - Window server 2022
    - OPNsense
    - Windows 10   
    
## 3. Needed Hardware
 * Server 1
 * Server 2
 * ClientPC windows 10
 * OPNsense Firewall

## 4. Step-by-step guide

1. Open hyper-v

2. Click on ``Virtual Switch Manager`` 
    - Select ``New Virtual Network Switch``
    - select **External** , and click ``Create Virtual Switch``, 
    - Name the switch **WAN**
    - For Connection type Choose ``External Network`` then ``Realtek PCIe GbE Family Controller``
    - Click apply
    - Click Ok

3. Click on **New** Then ``Virtual Machine`` 
    - **Specify Name and Location**. Select the name for your VM (Virtual Machine) Then click ``Next``

4. **Specify Generation** 
    - Click on ``Generation 2`` then click **Next**

5. **Asign Memory** 
    - Type in ``2048`` or higher and click ``Next``

6. **Configure Networking**
    - Choose **WAN** and click ``Next``

7. **Connect Virtual Hard Disk**
    - For size, type 2GB. click **Next**

8. **Installation Options**
    - Select ``Install an operating system for a bootable image file``. Find the ``OPNsense ISO file`` and click **Finish**

9. **Summary** 
    - Click ``Finish``

10. Right click the new created VM and click ``Settings``

11. Find ``Add Hardware`` and add ``Network Adapter``, Then click ``Add``

12. In the new created Network Adapter choose **WAN**. After that, Click ``VLAN ID`` and type in your ID (*In this example i will be using 320. Your ID can be whatever you want.*) Then click **Apply**

13. Click ``Ok``    