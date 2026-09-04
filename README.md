# Enterprise Bank Network


In this project, I created an enterprise network for a bank. There are several VLANs (10-120) for different sections of the bank, including HR, accounting, managment, customer care, admin, etc. Multiple forms of redundancy were added, including multiple routers and switches in case one fails. One issue I ran into with this project was correctly assigning DHCP to some of the devices. Some of the devices were not getting IP addresses from the DHCP server and couldn't ping any other device, but the issue was some incorrect IP configurations with some of the switches.
