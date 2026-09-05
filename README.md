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

3. DHCP Server Configuration
Configured two DHCP pools for the network
<img width="680" height="555" alt="image" src="https://github.com/user-attachments/assets/51a11bba-50e8-41fd-9696-057c3e3a7e04" />
As you can see for pool switch0, the default gateway is 192.168.10.1 because that is the IP address given to the router interface that connects the switch to the router. The starting address
is 192.168.10.3 because the switch has the static address 192.168.10.2.

<img width="683" height="526" alt="image" src="https://github.com/user-attachments/assets/ea8b9f30-30e6-4d11-b7d8-c8d10185863c" />
Pretty much the same thing for pool switch1 except for the default gateway and the starting address being 192.168.20.2 because the only other static address is for the router interface.


5. Router Configuration


6. Testing
