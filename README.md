**# Set-up-a-basic-firewall
pfSense_**

What is pfSense? pfSense is a firewall/router computer software distribution based on FreeBSD.

Purpose? It is primarily used as a router and firewall software and is frequently set up as a DHCP server, DNS server, WiFi access point, and VPN server, all on the same physical device.

Installing pfSense In this repo, i will demonstrate how to set up pfsense for your home lab. This whole process will be set up on a virtual box and i will be using Ubuntu as the admin system and configuring the pfsense. In this repo, i will create rules in the firewall, configure VPN and monitor the rules.

1.Download & Install pfSense Visit the pfSense website to download the software:
Install it on a dedicated machine or try using VirtualBox if you're comfortable with virtual environments.

2. Initial Configuration:
Access pfSense via your browser by entering its local IP (typically 192.168.1.1). Log in using the default credentials (username: admin, password: pfsense).

4. Set Up Network Interfaces:
Assign the network interfaces: WAN (your internet connection) and LAN (your home network). Follow the setup wizard to configure these correctly.

6. Basic Firewall Rules:
Go to Firewall > Rules and set up these essential rules -
Allow LAN to WAN: Lets your devices access the internet.
Block WAN to LAN: Blocks any unwanted traffic from entering your network.

7. Test Your Firewall:
Ensure your firewall rules work by accessing the internet within your network. Test from an external source to verify that unauthorized access is blocked.

8. Monitor Traffic Logs:
Navigate to Status > System Logs > Firewall to monitor all incoming and outgoing traffic, showing what’s being blocked or allowed.
