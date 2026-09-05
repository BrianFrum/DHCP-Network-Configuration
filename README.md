# Enterprise Bank Network

-----Summary-----

This project involved setting up and configuring a simple logical network topology, which includes switches, endpoints, a router, and a server that will be used for DHCP. Network connectivity was also tested to make sure everything worked as intended.

-----Skills Demonstrated-----

- Configuration: Configured network devices (mainly server and router).
- Conectivity Testing: use ping to make sure every device can communicate.


-----Technologies Used-----

- CISCO Packet Tracer


-----Project Walkthrough-----

1. Logical Topology Setup
Drag and drop everything needed for the network
<img width="1272" height="601" alt="image" src="https://github.com/user-attachments/assets/7f93be03-ab88-4deb-8a17-333dec2da8bf" />


2. DHCP Server Configuration
Configured two DHCP pools for the network

As you can see for pool switch0, the default gateway is 192.168.10.1 because that is the IP address given to the router interface that connects the switch to the router. The starting address
is 192.168.10.3 because the switch has the static address 192.168.10.2.
<img width="680" height="555" alt="image" src="https://github.com/user-attachments/assets/51a11bba-50e8-41fd-9696-057c3e3a7e04" />

Pretty much the same thing for pool switch1 except for the default gateway and the starting address being 192.168.20.2 because the only other static address is for the router interface.
<img width="683" height="526" alt="image" src="https://github.com/user-attachments/assets/ea8b9f30-30e6-4d11-b7d8-c8d10185863c" />

To make sure each network can communicate with each other, the default serverpool in the DHCP service needs to have the default gateway set to the default gateway of the network. In this case it is 192.168.10.1.
If the server was in the other network it would be 912.18.20.1
<img width="775" height="519" alt="image" src="https://github.com/user-attachments/assets/e4b03af8-5be8-490d-bd26-68696df13245" />


3. Router Configuration
First, configured the connected interfaces with their appropiate IP addresses, 192.168.10.1 and 192.18.20.1. Also, an ip-helper address for each interface, which is 192.168.10.2 (the static IP address of the server).
<img width="1051" height="832" alt="image" src="https://github.com/user-attachments/assets/ee61eda8-bf96-4c5a-a8ae-33df6cdb2fa3" />


4. Testing
Go into each endpoint, select desktop, select IP Configuration, and select DHCP. If everything works, the IP address will be automatically assigned with DHCP
<img width="690" height="701" alt="image" src="https://github.com/user-attachments/assets/1de395bb-1638-419c-a4f2-a848d2d44d5d" />


In the command prompt of any computer, ping a device in the same network, the other network, and the router. If everything work you should get a reply from each.
<img width="785" height="724" alt="image" src="https://github.com/user-attachments/assets/2343ba12-f1b6-4a2b-b39e-bf89e6076c4d" />
