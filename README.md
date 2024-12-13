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

### 1. Open hyper-v


2. Click on ``Virtual Switch Manager`` Select ``New Virtual Network Switch`` and select **External** , and click ``Create Virtual Switch``, 

    - Name the switch **WAN**
    - Connection type Choose ``External Network`` then ``Realtek PCIe GbE Family Controller``
    - Click apply
    - Click Ok

3. Click on **New** Then ``Virtual Machine`` Select next, Then choose a name for your Virtual Machine
    - Click next until ur on the page of **Specify Name and Location**. In here you will Name your machine then click ``Next``
    - in Specify Generation click on ``Generation 2`` then click next