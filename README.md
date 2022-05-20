Design and configure network for Acme Ltd. Use real equipment on Lab KMD658. Switch2 and labrouter are preconfigured. 
Connection to labnetwork is through RJ45 connectors named Labnetwork 10.95.0.0/23).
 
<img width="619" alt="Screenshot 2022-05-20 at 21 30 31" src="https://user-images.githubusercontent.com/76178825/169590875-0cc38571-0a25-4de1-9ab8-16fcee5c801f.png">


1.	Use Per Vlan Spanninnig tree plus as Spanning Tree protocol
2.	Routing protocol used in this Case Study is single area OSPF
3.	Configure parallel Ethernet links as Etherchannels
4.	Configure all used device connected ports as access ports with port security enabled and configure as spanning tree edge ports. Portsecurity violation should cause the port to shutdown state. 
5.	There are following types of users (Staff, Students, Management and Guest) that need to be connected to separate VLANS. Prepare to have at least 300 users in Students VLAN. For VLANs you can use following IP address range 10.95.X[0-9].0 where X is the POD number (1-14)u 
6.	In every VLAN there has to be a DHCP server. Reserve 32 IP-addreses in each VLAN for devices with static IP addresses 
7.	Configure NTP to synchronize clocks between Switches and end devices and configure also correct time zones  (EET) and also summertime transition rules (EEST).  Configure two NTP servers: 10.94.1.3 and 10.94.4.254) 
8.	All access-ports must be configured with portfast and BPDU-guard and port security with only two mac addresses allowed per port. 
9.	Configure all switches to support SSH and disable telnet to them. For login authentication on switches configure all switches to use local database (database must have a user cisco with password ciscoeigrp configured). 
10.	Limit remote management connections only from devices in MGT VLAN
11.	Configure SSH to use version 2.

Test your implementation of case study and write a report where you explain how the requirements were configured to devices (what command were used and their possible limitations ) and also explain how and what test were performed and any shortcomings found during testing. Include all configurations from all network devices as appendix to your report. Answer questions presented at the end of this case study. 



Questions: 
1.	How many links will DS1 see in spanning-tree?
2.	Where there any requirements in this Case Study that you were unable to fulfill?
3.	How you could improve security and performance of the network in your implementation of case study
4.	How much time did  this Case Study take?
