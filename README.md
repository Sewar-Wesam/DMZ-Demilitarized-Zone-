# DMZ ( Demilitarized Zone )
Unlock your knowledge 

## What is DMZ?   
DMZ typically is a VLAN ( Virtual LAN ) instead of physical network. DMZ can be considered as a separate subnetwork, it is used to host the services that need to be accessable from the internet like ( Web, Email, DNS ).  
## Why do we use DMZ?   
In general, DMZ is used for two main goals:   
- Isolation: To isolate the internal network from the public servers, this will prevent from the risk if the public servers are compromised.
- Security : DMZ adds layer of security, so if the attackers breach a server in DMZ, he needs to check another measures like Firewall's rule table to access the internal network.

### Let us walk through this example: 

![image](https://github.com/user-attachments/assets/d876c5b7-e552-4897-a122-58219a36c13e)

#### We want to answer this question: How Traffic Flows in a DMZ Topology  
- The inbound traffic is the traffic comming from the internet to the DMZ.
- Firewall permits the traffic that is comming from internet to the DMZ, but blocking it from the internal network resources.
- The firewall allows this traffic but monitors it for quastionable activity.
- If DMZ wants to communicate with the internal network, then the firewall restricts with predefined rules to allow only the necessary communications to take place. 

