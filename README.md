<h1>Packet-Tracer-Network-Setup-Star-Ring-Vlan-Project</h1>


<h2>Description</h2>
This project demonstrates the configuration and analysis of network devices using Cisco Packet Tracer. It includes the design and setup of scalable star and ring topologies with VLAN segmentation. The project simulates real-world network behavior by modeling data flow between devices and verifying connectivity and VLAN functionality. This hands-on exercise reinforces key networking concepts and basic device configuration skills.
<br />


<h2>Languages and Utilities Used</h2>

- Cisco Packet Tracer – For simulating and configuring network devices and topologies
- Networking Protocols – VLAN, Ethernet, and switching concepts
- Star and Ring Topologies – For designing different network structures
- Basic Configuration Commands – To configure switches, VLANs, and verify connectivity (e.g., vlan, switchport, ip address, ping)
- Command-Line Interface (CLI) – For applying and testing network configurations

<h2>Environments Used </h2>

- Cisco Packet Tracer – For network simulation and device configuration
- Host OS: macOS Ventura 13.7.4

<h2>Program walk-through:</h2>

<p align="center">
Set up star topologies and configure VLANs. Launch Cisco Packet Tracer: <br/>
<img src="https://i.imgur.com/ZRUAO4Y.png"/>
<br />
<br />
Select 2960-24TT switch and drag it to the main screen:  <br/>
<img src="https://i.imgur.com/Th4ubMg.png"/>
<br />
<br />
Click on End Devices located at the bottom left then drag and drop four PCs onto the workspace: PC0, PC1, PC2, and PC3: <br/>
<img src="https://i.imgur.com/FsrBLTI.png"/>
<br />
<br />
Click on Connections, select copper straight through cable. Now click on the Switch and select FastEthernet0/1 port, then click on PC0 and select FastEthernet0 port:  <br/>
<img src="https://i.imgur.com/BnjZxwJ.png"/>
<img src="https://i.imgur.com/flrhUi5.png"/>
<br />
<br />
Repeat the process for PC1, PC2 and PC3. First, connect the switch's FastEthernet0/2 port to PC1's FastEthernet0 port, connect the switch's FastEthernet0/3 to PC2's FastEthernet0 then connect the switch's FastEthernet0/4 to PC3's FastEthernet0:  <br/>
<img src="https://i.imgur.com/VaZz6AU.png"/>
<br />
<br />
Now click on Wireless Devices located at the bottom left, drag and drop a Home Router Wireless Router onto the workspace:  <br/>
<img src="https://i.imgur.com/3WDc4G4.png"/>
<br />
<br />
Click on Connections, select Copper Cross-Over Cable, click on the Router and select GigabitEthernet 1 port, then click on Switch and select FastEthernet0/5 port:  <br/>
<img src="https://i.imgur.com/aRU0PuT.png"/>
<img src="https://i.imgur.com/kaKGxCl.png"/>
<br />
<br />
Click on PC0 to assign an IP address to the PC, select Desktop, IP Configuration, then select DHCP to automatically assign an IP address:  <br/>
<img src="https://i.imgur.com/CdiG76a.png"/>
<br />
<br />
Repeat the process for PC1, PC2 and PC3:  <br/>
<img src="https://i.imgur.com/E2mLhdC.png"/> 
<br />
<br />
To check the connectivity, click on the PC0, select Desktop, then Command Prompt and use the following commands ping 192.168.0.101 ping 192.168.0.102 ping 192.168.0.103:  <br/>
<img src="https://i.imgur.com/EJ9X2Kx.png"/>
<br />
<br />
Create a ring topology and configure VLANs. Click on End Devices at the bottom left, then drag and drop four PCs onto the workspace: PC4, PC5, PC6, and PC7, arranging them in a circular formation:  <br/>
<img src="https://i.imgur.com/SAANEAI.png"/>
<br />
<br />
Click on Network Devices, then drag 4 Switches to the center of the PC's ring formation:  <br/>
<img src="https://i.imgur.com/xuKUCdN.png"/>
<br />
<br />
Click on Connections, Select Copper Cross-Over cable, then connect each PC to a different switch:
  
• PC1: Connect PC1's FastEthernet0 port to Switch1's FastEthernet0/1 port

• PC2: Connect PC2's FastEthernet0 port to Switch2's FastEthernet0/1 port

• PC3: Connect PC3's FastEthernet0 port to Switch3's FastEthernet0/1 port

• PC4: Connect PC4's FastEthernet0 port to Switch4's FastEthernet0/1 port:  <br/>
<img src="https://i.imgur.com/lJonfrv.png"/>
<br />
<br />
Now, connect the switches in a circular (ring) manner using Copper Cross-Over cables:

• Connect Switch1's FastEthernet0/2 to Switch2's FastEthernet0/2

• Connect Switch2's FastEthernet0/3 to Switch3's FastEthernet0/2

• Connect Switch3's FastEthernet0/3 to Switch4's FastEthernet0/2

• Finally, connect Switch4's FastEthernet0/3 back to Switch1's FastEthernet0/3,
completing the ring:  <br/>
<img src="https://i.imgur.com/Y0LGile.png"/>
<br />
<br />
Click on PC4, go to the Desktop tab, and open IP Configuration, then assign the following Static IP address and subnet mask: 

• PC4: IP 192.168.20.2, Subnet Mask 255.255.255.0:  <br/>
<img src="https://i.imgur.com/EC4IMwY.png"/>
<br />
<br />
Repeat the steps for the remaining 3PCs:

• PC5: IP 192.168.20.3, Subnet Mask 255.255.255.0

• PC6: IP 192.168.20.4, Subnet Mask 255.255.255.0

• PC7: IP 192.168.20.5, Subnet Mask 255.255.255.0: <br/>
<img src="https://i.imgur.com/wQfQvdk.png"/>
<br />
<br />
Now to verify connectivity:

• On PC4, go to the Desktop tab and open the Command Prompt

• Type ping 192.168.20.3 to check connectivity with PC2

• Type ping 192.168.20.4 to check connectivity with PC3

• Type ping 192.168.20.5 to check connectivity with PC4

• Repeat the same on the other PCs to ensure that all devices can ping each other:<br/>
<img src="https://i.imgur.com/e1sfdyz.png"/>
<br />
<br />
Great! You've successfully designed, configured, and tested star and ring network topologies with VLANs — a solid step forward in mastering network infrastructure:  <br/>
<img src="https://i.imgur.com/FZ0SiYx.png"/>
<br />
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
